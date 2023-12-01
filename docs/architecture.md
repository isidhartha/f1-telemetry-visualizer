# Architecture — F1 Telemetry Visualizer

## Overview

F1 Telemetry Visualizer is a layered desktop application. The user interacts with a terminal-based CLI that drives session selection, which in turn fetches and processes real F1 telemetry from the FastF1 library and renders the results in a native PySide6 desktop window. The three principal layers — CLI, data, and visualization — are intentionally kept loosely coupled so that each can evolve independently.

---

## Component Breakdown

### CLI Layer

The CLI layer is built with **Questionary** for interactive prompts (season, round, session type, driver selection) and **Rich** for formatted terminal output. It is the single entry point to the application. When the user confirms their selection, the CLI layer passes a structured configuration object to the data layer and hands off control to the visualizer.

The CLI layer has no knowledge of how data is fetched or how charts are drawn. It only collects user intent and triggers downstream processing.

### Data Layer

The data layer wraps **FastF1** to load session objects from the official F1 timing archive. Raw session data is cached to disk (configurable via `FASTF1_CACHE_DIR`) so that repeated runs do not re-download the same session. Once loaded, **Pandas** DataFrames are used to align telemetry channels across laps and drivers, normalize sample rates, and derive computed channels such as braking events, DRS state transitions, and compound stint boundaries.

The data layer exposes a clean interface (`load_session()`, `get_lap_telemetry()`, `compare_drivers()`) consumed by the visualization layer. It performs no rendering of its own.

### Visualization Layer

The visualization layer is split between **Matplotlib** (static and animated charts — speed traces, throttle/brake overlays, multi-driver comparisons) and **Arcade** (the animated circuit map that shows car positions during replay). Both are embedded inside a **PySide6** application window, which provides the main event loop, layout management, and user controls (play, pause, scrub, lap selector).

---

## Data Flow

```
User Input (CLI)
      |
      v
FastF1 API  -->  Disk Cache
      |
      v
Pandas Data Processor
  - Telemetry alignment
  - Compound / DRS derivation
      |
      v
Visualizer (Matplotlib + Arcade)
      |
      v
PySide6 Window (rendered to screen)
```

Session data is loaded once per run and held in memory. The replay scrubber slices the in-memory DataFrame by lap and timestamp, feeding frames to both the chart renderer and the circuit map at a configurable playback rate.
