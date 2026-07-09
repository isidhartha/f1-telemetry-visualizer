# F1 Telemetry Visualizer — Roadmap

Since launching this project I've received a lot of feedback and feature requests from people in the F1 data community. This roadmap captures where the project is headed so that anyone wanting to contribute or build on top of it knows what to expect.

## Vision

The goal is to make this the most capable open-source tool for exploring F1 telemetry data. That means a rich, interactive experience — not just static charts, but something that lets you replay sessions lap by lap, compare drivers side-by-side, and dig into the numbers the way a race engineer would. Your own personal pit wall.

## Primary Goals

- **GUI Menu System** — A proper graphical interface for navigating race weekends, sessions, and drivers. Currently in progress; the goal is to replace the interactive terminal prompt with a full PySide6 window.
- **Race Insight Charts** — An extended suite of visualisations covering tyre strategy, track evolution, pit stop deltas, and driver performance trends across a full stint.
- **Practice Session Support** — Expand beyond qualifying and race to include FP1/FP2/FP3. The approach will combine the telemetry analysis used for qualifying with the track-position replay used for race mode.

## Performance and UX Improvements

As the feature set grows, performance stays a priority:

- **Reduce replay lag** — The rendering pipeline needs optimisation for lower-end machines. Particular focus on the race replay where multiple overlays are drawn simultaneously.
- **Declutter the UI** — Better toggle controls and preset view modes so users can focus on the data that matters without the interface getting overwhelming.
- **Faster session loading** — Investigate smarter FastF1 cache strategies and lazy-loading of telemetry channels that aren't immediately visible.

## Planned Features

- Tyre degradation model overlay
- Sector-by-sector time loss analysis
- Weather and track temperature timeline
- Export to shareable HTML report

## Contributing

If you want to help bring any of these features to life, feel free to open an issue or submit a pull request. Contributions of any size are welcome — whether that's a bug fix, a new chart type, or performance work.

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.
