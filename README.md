# F1 Telemetry Visualizer

A desktop application that replays Formula 1 race and qualifying sessions as animated, real-time visualizations. Pick any race from 2018 onwards from the GUI session selector, load the telemetry via FastF1, and watch all 20 drivers move around the track simultaneously — with DRS zones highlighted, safety car periods animated, and pit stops flagged per driver on the leaderboard. A secondary insights panel gives you live telemetry streams, tyre strategy timelines, gap charts, and race control messages alongside the replay.

The processing pipeline runs each driver's telemetry in parallel using `multiprocessing.Pool`, resamples everything onto a shared 25 FPS timeline, and caches the result as a pickle file. Subsequent loads of the same session skip the processing entirely. The replay engine itself uses the `arcade` library for the animated track map, with PySide6 windows for the GUI session selector and all the floating insight panels.

Qualifying sessions get their own replay mode with Q1/Q2/Q3 segment handling and per-driver fastest lap overlays. Sprint weekends are supported too — the CLI flags `--sprint` and `--sprint-qualifying` select the right session type.

## Features

- **PySide6 GUI session selector** — tree-view browser for the full F1 calendar from 2018, filterable by year and race name, with buttons for Race, Sprint, Qualifying, and Sprint Qualifying
- **Arcade 2D replay window** — animated 25 FPS track map showing all drivers simultaneously using official team colors
- **Parallel telemetry processing** — `multiprocessing.Pool` processes each driver's data concurrently and resamples onto a shared frame timeline
- **Safety car physics simulation** — computes safety car position frame by frame through deploying, on-track, and returning phases using KD-tree spatial lookups for smooth animation
- **DRS zone detection** — prefers qualifying lap for accurate DRS data; falls back to fastest race lap with speed-based detection when qualifying isn't available
- **Pit stop integration** — PitInTime and PitOutTime extracted per driver and injected into every replay frame for leaderboard display
- **Weather data overlay** — track temperature, air temperature, humidity, wind speed, wind direction, and rain state resampled and attached to each frame
- **Race control feed** — FIA messages (flags, penalties, safety car, DRS notices, sector alerts) parsed and time-synchronized to the replay timeline
- **Qualifying replay mode** — separate animated screen for Q sessions with Q1/Q2/Q3 segment handling and per-driver fastest-lap telemetry
- **Insights menu** — secondary floating PySide6 window with six panels: Driver Live Telemetry, Live Tyre Strategy, Track Position Map, Race Control Feed, Lap Time and Gap Chart, Telemetry Stream Viewer
- **Pickle cache** — computed telemetry saved to `computed_data/`; use `--refresh-data` to force a fresh download and reprocess
- **CLI mode** — `--cli` bypasses the GUI for headless or scripted usage; `--no-hud` hides the overlay for a clean track view

## Tech Stack

| Library | Purpose |
|---|---|
| `fastf1` | Official F1 telemetry and session data |
| `pandas` | Data manipulation and lap filtering |
| `numpy` | Array resampling and timeline construction |
| `arcade` | 2D animated replay window |
| `pyside6` | GUI session selector and insights panels |
| `matplotlib` | Supplementary plotting in insight windows |
| `questionary` | Interactive CLI session picker |
| `rich` | Terminal output formatting |

## Setup

```bash
git clone https://github.com/isidhartha/f1-telemetry-visualizer.git
cd f1-telemetry-visualizer
pip install -r requirements.txt
python main.py
```

This opens the PySide6 session selector. Pick a year and race weekend from the tree, then click a session button to load the telemetry and launch the replay.

**CLI usage:**

```bash
# List rounds for a year
python main.py --list-rounds --year 2024

# Launch race replay directly
python main.py --viewer --year 2024 --round 5

# Qualifying session
python main.py --viewer --year 2024 --round 5 --qualifying

# Sprint race
python main.py --viewer --year 2024 --round 5 --sprint

# Sprint qualifying
python main.py --viewer --year 2024 --round 5 --sprint-qualifying

# Hide HUD overlay
python main.py --viewer --year 2024 --round 5 --no-hud

# Force re-download of session data
python main.py --viewer --year 2024 --round 5 --refresh-data
```

## Architecture

```mermaid
flowchart TD
    A([python main.py]) --> B{Launch mode}
    B -- no flags --> C[RaceSelectionWindow\nPySide6 GUI]
    B -- --viewer --> D[main function]
    B -- --cli --> E[cli_load]
    C -- user picks session --> D

    D -- Race/Sprint --> F[get_race_telemetry\nfastf1 + multiprocessing]
    D -- Qualifying --> G[get_quali_telemetry\nfastf1 + multiprocessing]

    F --> H[_compute_safety_car_positions\nKD-tree per frame]
    F --> I[Pickle cache\ncomputed_data/]
    I --> J[run_arcade_replay\n25 FPS animated map]

    G --> K[Pickle cache\ncomputed_data/]
    K --> L[run_qualifying_replay\nQ1/Q2/Q3 segments]

    J --> M[launch_insights_menu\nPySide6 floating panel]
    M --> N1[Driver Telemetry]
    M --> N2[Tyre Strategy]
    M --> N3[Track Position]
    M --> N4[Race Control Feed]
    M --> N5[Lap Time Chart]
    M --> N6[Telemetry Stream Viewer]
```

## Demo

> Screenshots coming soon.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

MIT

## Author

[isidhartha](https://github.com/isidhartha)
