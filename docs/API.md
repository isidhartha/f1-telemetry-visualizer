# Module API — F1 Telemetry Visualizer

This application is a desktop tool with no HTTP server. The "API" described here is the internal Python module interface — the functions other modules call to load data, trigger replay, and render charts. All public functions live under the `src/` package.

---

## `data.loader`

### `load_session(year: int, round: int, session_type: str) -> fastf1.core.Session`

Loads and caches a FastF1 session object. `session_type` accepts `"R"` (race), `"Q"` (qualifying), `"FP1"`, `"FP2"`, `"FP3"`. Raises `SessionNotAvailableError` if the requested session does not exist in the FastF1 archive.

### `get_lap_telemetry(session, driver: str, lap_number: int) -> pd.DataFrame`

Returns a DataFrame of telemetry channels — `Speed`, `Throttle`, `Brake`, `DRS`, `nGear`, `Distance` — for the specified driver and lap. Channels are resampled to a uniform 10 Hz grid.

### `compare_drivers(session, drivers: list[str], lap_numbers: list[int]) -> dict[str, pd.DataFrame]`

Returns a dict keyed by driver code. Each value is the aligned telemetry DataFrame for that driver's requested lap, distance-normalized so that all drivers share the same x-axis.

---

## `replay.controller`

### `replay(session, driver: str, speed: float = 1.0) -> None`

Starts the PySide6 replay window for the given session and driver. `speed` is a playback multiplier (e.g. `2.0` plays at double speed). Blocks until the window is closed.

---

## `viz.charts`

### `plot_speed_trace(telemetry: pd.DataFrame, ax: matplotlib.axes.Axes | None = None) -> matplotlib.figure.Figure`

Renders a speed-vs-distance line chart onto `ax`. If `ax` is `None`, a new figure is created. Returns the Figure for embedding in PySide6 or saving to disk.

### `plot_comparison(driver_data: dict[str, pd.DataFrame], channels: list[str]) -> matplotlib.figure.Figure`

Renders a multi-panel comparison figure. Each panel corresponds to one telemetry channel. Drivers are colour-coded automatically.

---

## `viz.circuit`

### `draw_circuit_map(session, lap_number: int) -> arcade.Window`

Opens an Arcade window rendering the circuit outline with car position markers for the given lap.
