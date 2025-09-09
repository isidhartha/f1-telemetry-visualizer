# Changelog

All notable changes are documented here.


### 2022-01-09
- perf: reduce peak memory in multi-driver comparison


### 2022-01-10
- fix: handle DNF laps in multi-driver comparison mode


### 2022-01-13
- style: normalise import ordering with isort


### 2022-01-14
- feat: implement batch circuit map export for all drivers


### 2022-01-17
- feat: implement session selection via interactive prompt


### 2022-01-18
- feat: implement interpolated distance axis for alignment


### 2022-02-03
- fix: correct time alignment when laps share same timestamp


### 2022-02-13
- feat: implement synthetic lap data fallback for CI


### 2022-02-16
- feat: add gear trace visualization alongside speed profile


### 2022-02-18
- refactor: rename ambiguous variables in lap parser module


### 2022-02-20
- test: add unit tests for lap time parser


### 2022-02-20
- chore: clean up unused imports across modules


### 2022-02-22
- test: add unit tests for lap time parser


### 2022-02-22
- fix: correct sector boundary detection for specific circuits


### 2022-02-23
- feat: add gear trace visualization alongside speed profile


### 2022-02-24
- feat: add FastF1 session loader with local cache support


### 2022-03-01
- test: add tests for telemetry alignment edge cases


### 2022-03-02
- test: add regression test for DNF lap exclusion logic


### 2022-03-11
- test: add WebSocket broadcast unit tests


### 2022-03-20
- fix: handle DNF laps in multi-driver comparison mode


### 2022-03-22
- refactor: extract all constants to config module


### 2022-03-24
- perf: reduce peak memory in multi-driver comparison


### 2022-03-27
- feat: add configurable FastF1 cache dir via environment


### 2022-03-29
- feat: add gear trace visualization alongside speed profile


### 2022-04-01
- feat: add lap time delta chart between selected drivers


### 2022-04-09
- refactor: simplify telemetry alignment with vectorised ops


### 2022-04-12
- docs: update architecture diagram in docs/architecture.md


### 2022-04-12
- fix: handle FastF1 API rate limit with backoff


### 2022-04-13
- feat: implement weather condition overlay on race charts


### 2022-04-13
- test: add regression test for DNF lap exclusion logic


### 2022-04-18
- feat: implement synthetic lap data fallback for CI


### 2022-04-19
- chore: add pre-commit hooks for black and ruff


### 2022-04-27
- fix: correct DRS detection for Monaco street circuit


### 2022-05-03
- refactor: rename ambiguous variables in lap parser module


### 2022-05-09
- refactor: split large render function into focused helpers


### 2022-05-10
- feat: add rich terminal UI with live leaderboard display


### 2022-05-13
- style: fix line length violations in visualizer module


### 2022-05-16
- feat: implement session selection via interactive prompt


### 2022-05-21
- refactor: rename ambiguous variables in lap parser module


### 2022-05-24
- feat: add FastF1 session loader with local cache support


### 2022-05-25
- feat: add multi-driver telemetry comparison overlay


### 2022-05-30
- fix: handle missing pit stop data in cached sessions


### 2022-05-31
- feat: add compound strategy timeline for full race


### 2022-06-03
- feat: implement lap telemetry parser for speed and throttle channels


### 2022-06-03
- feat: add CSV export for aligned telemetry channels


### 2022-06-07
- refactor: replace manual loop with pandas apply in parser


### 2022-06-16
- feat: implement weather condition overlay on race charts


### 2022-06-27
- fix: correct DRS detection for Monaco street circuit


### 2022-06-27
- feat: add lap time delta chart between selected drivers


### 2022-06-28
- refactor: simplify telemetry alignment with vectorised ops


### 2022-06-30
- fix: handle timezone offset in session timestamp parsing


### 2022-07-02
- feat: add CSV export for aligned telemetry channels


### 2022-07-04
- feat: implement sector time breakdown visualization panel


### 2022-07-07
- feat: implement tyre compound colour coding on traces


### 2022-07-11
- docs: add circuit map colour legend documentation


### 2022-07-13
- fix: fix matplotlib display on headless CI environments


### 2022-07-21
- fix: fix incorrect lap count when VSC period is active


### 2022-07-23
- docs: update installation steps for Windows users


### 2022-07-24
- fix: handle missing telemetry for early 2022 season races


### 2022-07-25
- chore: add fastf1_cache to .gitignore


### 2022-07-28
- fix: handle timezone offset in session timestamp parsing


### 2022-07-29
- perf: reduce peak memory in multi-driver comparison


### 2022-07-29
- refactor: consolidate session loading into utility class


### 2022-08-06
- chore: clean up unused imports across modules


### 2022-08-08
- test: add unit tests for lap time parser


### 2022-08-08
- docs: update installation steps for Windows users


### 2022-08-08
- test: add regression test for DNF lap exclusion logic


### 2022-08-10
- fix: fix matplotlib display on headless CI environments


### 2022-08-12
- feat: implement DRS zone detection from car data channels


### 2022-08-15
- fix: fix matplotlib display on headless CI environments


### 2022-08-17
- refactor: extract circuit map renderer to separate class


### 2022-08-24
- feat: implement multi-client WebSocket fan-out server


### 2022-08-26
- fix: correct DRS detection for Monaco street circuit


### 2022-08-30
- refactor: consolidate session loading into utility class


### 2022-09-02
- fix: resolve encoding issue in non-ASCII driver name display


### 2022-09-04
- fix: handle missing pit stop data in cached sessions


### 2022-09-10
- feat: implement circuit map with racing line overlay


### 2022-09-21
- fix: fix interpolation edge case at lap start boundary


### 2022-09-25
- feat: implement live WebSocket broadcast for session data


### 2022-09-27
- test: add regression test for DNF lap exclusion logic


### 2022-09-27
- fix: handle missing pit stop data in cached sessions


### 2022-09-29
- fix: correct sector boundary detection for specific circuits


### 2022-09-30
- test: add tests for telemetry alignment edge cases


### 2022-09-30
- feat: add FastF1 session loader with local cache support


### 2022-10-04
- style: format all source files with black


### 2022-10-05
- test: add tests for telemetry alignment edge cases


### 2022-10-07
- feat: implement tyre compound colour coding on traces


### 2022-10-10
- fix: fix interpolation edge case at lap start boundary


### 2022-10-16
- feat: add rich terminal UI with live leaderboard display


### 2022-10-18
- fix: fix incorrect lap count when VSC period is active


### 2022-10-27
- perf: reduce peak memory in multi-driver comparison


### 2022-10-27
- test: add WebSocket broadcast unit tests


### 2022-10-28
- perf: reduce peak memory in multi-driver comparison


### 2022-11-08
- fix: handle timezone offset in session timestamp parsing


### 2022-11-15
- fix: correct time alignment when laps share same timestamp


### 2022-11-15
- fix: correct tyre compound mapping for 2022 season codes


### 2022-11-29
- fix: resolve crash when selected driver has zero valid laps


### 2022-12-06
- feat: implement lap telemetry parser for speed and throttle channels


### 2022-12-09
- docs: update FastF1 cache configuration guide


### 2022-12-13
- docs: add circuit map colour legend documentation


### 2022-12-16
- fix: resolve NaN values in telemetry alignment step


### 2022-12-16
- feat: add automatic reconnection for dropped clients


### 2022-12-19
- refactor: simplify telemetry alignment with vectorised ops


### 2022-12-19
- fix: resolve encoding issue in non-ASCII driver name display


### 2022-12-22
- chore: clean up unused imports across modules


### 2022-12-28
- docs: add lap comparison usage examples to README


### 2022-12-28
- fix: handle missing pit stop data in cached sessions


### 2022-12-29
- perf: reduce peak memory in multi-driver comparison


### 2023-01-03
- refactor: simplify telemetry alignment with vectorised ops


### 2023-01-06
- refactor: split large render function into focused helpers


### 2023-01-06
- feat: add automatic reconnection for dropped clients


### 2023-01-08
- feat: add compound strategy timeline for full race


### 2023-01-09
- chore: add fastf1_cache to .gitignore


### 2023-01-11
- feat: implement interpolated distance axis for alignment


### 2023-01-19
- chore: clean up unused imports across modules


### 2023-01-22
- chore: update FastF1 dependency to 3.3.x


### 2023-01-23
- feat: implement batch circuit map export for all drivers


### 2023-01-26
- feat: add gear trace visualization alongside speed profile


### 2023-01-27
- refactor: extract circuit map renderer to separate class


### 2023-01-30
- fix: correct lap time parsing for sector 3 edge case


### 2023-01-30
- feat: implement live WebSocket broadcast for session data


### 2023-02-02
- feat: implement sector time breakdown visualization panel


### 2023-02-02
- test: add tests for telemetry alignment edge cases


### 2023-02-06
- chore: clean up unused imports across modules


### 2023-02-07
- feat: implement session selection via interactive prompt


### 2023-02-07
- chore: add pre-commit hooks for black and ruff


### 2023-02-08
- refactor: extract telemetry loading into dedicated module


### 2023-02-13
- docs: add circuit map colour legend documentation


### 2023-02-15
- feat: add multi-driver telemetry comparison overlay


### 2023-02-15
- docs: add lap comparison usage examples to README


### 2023-02-18
- feat: implement circuit map with racing line overlay


### 2023-02-23
- refactor: extract telemetry loading into dedicated module


### 2023-02-28
- chore: add fastf1_cache to .gitignore


### 2023-02-28
- perf: reduce peak memory in multi-driver comparison


### 2023-03-02
- feat: implement brake pressure overlay on lap comparison


### 2023-03-02
- feat: implement synthetic lap data fallback for CI


### 2023-03-10
- fix: correct sector boundary detection for specific circuits


### 2023-03-11
- fix: handle missing telemetry for early 2022 season races


### 2023-03-16
- chore: clean up unused imports across modules


### 2023-03-23
- feat: implement sector time breakdown visualization panel


### 2023-03-27
- fix: handle FastF1 API rate limit with backoff


### 2023-04-01
- refactor: separate visualization from data processing logic


### 2023-04-04
- feat: implement sector time breakdown visualization panel


### 2023-04-04
- feat: add CSV export for aligned telemetry channels


### 2023-04-06
- refactor: consolidate session loading into utility class


### 2023-04-06
- fix: resolve crash when selected driver has zero valid laps


### 2023-04-06
- fix: resolve NaN values in telemetry alignment step


### 2023-04-07
- feat: add fastest lap highlight across all drivers


### 2023-04-11
- fix: correct DRS detection for Monaco street circuit


### 2023-04-11
- test: add integration test with cached 2023 session data


### 2023-04-12
- feat: implement multi-client WebSocket fan-out server


### 2023-04-18
- fix: resolve crash when selected driver has zero valid laps


### 2023-04-29
- feat: implement circuit map with racing line overlay


### 2023-04-29
- feat: add session selector for race qualifying and practice


### 2023-05-05
- fix: correct time alignment when laps share same timestamp


### 2023-05-07
- feat: add FastF1 session loader with local cache support


### 2023-05-09
- chore: add fastf1_cache to .gitignore


### 2023-05-10
- feat: add gear trace visualization alongside speed profile


### 2023-05-11
- refactor: consolidate session loading into utility class


### 2023-05-14
- fix: resolve encoding issue in non-ASCII driver name display


### 2023-05-18
- feat: implement live WebSocket broadcast for session data


### 2023-05-28
- refactor: consolidate session loading into utility class


### 2023-05-30
- feat: implement live WebSocket broadcast for session data


### 2023-05-30
- fix: handle FastF1 API rate limit with backoff


### 2023-05-30
- perf: reduce peak memory in multi-driver comparison


### 2023-06-10
- chore: clean up unused imports across modules


### 2023-06-15
- fix: resolve NaN values in telemetry alignment step


### 2023-06-22
- refactor: extract circuit map renderer to separate class


### 2023-06-23
- fix: resolve encoding issue in non-ASCII driver name display


### 2023-06-23
- refactor: split large render function into focused helpers


### 2023-06-24
- chore: add fastf1_cache to .gitignore


### 2023-06-28
- refactor: simplify telemetry alignment with vectorised ops


### 2023-07-03
- fix: resolve encoding issue in non-ASCII driver name display


### 2023-07-11
- fix: correct lap time parsing for sector 3 edge case


### 2023-07-13
- feat: add automatic reconnection for dropped clients


### 2023-07-13
- test: add regression test for DNF lap exclusion logic


### 2023-07-18
- refactor: replace manual loop with pandas apply in parser


### 2023-07-18
- docs: update installation steps for Windows users


### 2023-07-19
- feat: add rich terminal UI with live leaderboard display


### 2023-07-23
- fix: handle DNF laps in multi-driver comparison mode


### 2023-07-26
- docs: add troubleshooting section for headless display


### 2023-07-27
- fix: fix matplotlib display on headless CI environments


### 2023-07-27
- fix: correct lap time parsing for sector 3 edge case


### 2023-08-01
- feat: implement DRS zone detection from car data channels


### 2023-08-03
- refactor: split large render function into focused helpers


### 2023-08-03
- fix: handle missing pit stop data in cached sessions


### 2023-08-03
- refactor: extract all constants to config module


### 2023-08-09
- feat: implement circuit map with racing line overlay


### 2023-08-13
- feat: add rich terminal UI with live leaderboard display


### 2023-08-16
- perf: reduce peak memory in multi-driver comparison


### 2023-08-24
- style: fix line length violations in visualizer module


### 2023-08-27
- feat: implement driver pace heatmap by lap


### 2023-08-28
- fix: handle missing telemetry for early 2022 season races


### 2023-09-02
- feat: implement synthetic lap data fallback for CI


### 2023-09-08
- refactor: replace manual loop with pandas apply in parser


### 2023-09-09
- feat: implement multi-client WebSocket fan-out server


### 2023-10-05
- refactor: move all plotting functions to visualizer module


### 2023-10-05
- feat: implement session selection via interactive prompt


### 2023-10-09
- fix: correct sector boundary detection for specific circuits


### 2023-10-13
- feat: add lap time delta chart between selected drivers


### 2023-10-16
- feat: implement DRS zone detection from car data channels


### 2023-10-20
- test: add integration test with cached 2023 session data


### 2023-10-24
- docs: document all telemetry column definitions and units


### 2023-10-25
- refactor: separate visualization from data processing logic


### 2023-11-03
- fix: resolve crash when selected driver has zero valid laps


### 2023-11-06
- refactor: extract circuit map renderer to separate class


### 2023-11-08
- docs: update FastF1 cache configuration guide


### 2023-11-08
- feat: implement weather condition overlay on race charts


### 2023-11-11
- feat: add gear trace visualization alongside speed profile


### 2023-11-13
- refactor: move all plotting functions to visualizer module


### 2023-11-14
- chore: pin pandas version for dtype compatibility


### 2023-11-14
- feat: add fastest lap highlight across all drivers


### 2023-11-16
- fix: correct tyre compound mapping for 2022 season codes


### 2023-11-20
- docs: document all telemetry column definitions and units


### 2023-11-23
- test: add integration test with cached 2023 session data


### 2023-11-28
- feat: add fastest lap highlight across all drivers


### 2023-11-28
- feat: implement live WebSocket broadcast for session data


### 2023-11-30
- fix: resolve crash when selected driver has zero valid laps


### 2023-12-01
- fix: handle missing pit stop data in cached sessions


### 2023-12-09
- feat: implement sector time breakdown visualization panel


### 2023-12-12
- fix: handle missing telemetry for early 2022 season races


### 2023-12-14
- style: format all source files with black


### 2023-12-14
- fix: correct time alignment when laps share same timestamp


### 2023-12-15
- fix: handle missing telemetry for early 2022 season races


### 2023-12-20
- test: add WebSocket broadcast unit tests


### 2023-12-21
- fix: fix incorrect lap count when VSC period is active


### 2024-01-03
- docs: update FastF1 cache configuration guide


### 2024-01-03
- fix: handle timezone offset in session timestamp parsing


### 2024-01-15
- feat: implement driver pace heatmap by lap


### 2024-01-17
- style: fix line length violations in visualizer module


### 2024-01-18
- feat: implement brake pressure overlay on lap comparison


### 2024-01-27
- docs: update installation steps for Windows users


### 2024-01-29
- feat: add configurable FastF1 cache dir via environment


### 2024-01-30
- feat: add rich terminal UI with live leaderboard display


### 2024-02-06
- feat: implement synthetic lap data fallback for CI


### 2024-02-08
- fix: correct lap time parsing for sector 3 edge case


### 2024-02-09
- fix: correct time alignment when laps share same timestamp


### 2024-02-13
- refactor: extract telemetry loading into dedicated module


### 2024-02-16
- fix: handle missing telemetry for early 2022 season races


### 2024-02-20
- perf: cache computed distance axis to avoid recomputation


### 2024-02-23
- docs: document all telemetry column definitions and units


### 2024-02-24
- docs: update FastF1 cache configuration guide


### 2024-03-02
- chore: add fastf1_cache to .gitignore


### 2024-03-04
- chore: add pre-commit hooks for black and ruff


### 2024-03-06
- feat: add gap-to-leader streaming in milliseconds


### 2024-03-06
- feat: implement sector time breakdown visualization panel


### 2024-03-09
- fix: fix matplotlib display on headless CI environments


### 2024-03-09
- feat: implement tyre compound colour coding on traces


### 2024-03-15
- feat: add multi-driver telemetry comparison overlay


### 2024-03-21
- feat: implement synthetic lap data fallback for CI


### 2024-03-22
- fix: handle DNF laps in multi-driver comparison mode


### 2024-03-22
- perf: reduce peak memory in multi-driver comparison


### 2024-03-25
- refactor: rename ambiguous variables in lap parser module


### 2024-03-26
- feat: implement interpolated distance axis for alignment


### 2024-03-27
- feat: add configurable FastF1 cache dir via environment


### 2024-03-29
- feat: implement circuit map with racing line overlay


### 2024-03-29
- test: add unit tests for lap time parser


### 2024-03-29
- docs: add lap comparison usage examples to README


### 2024-03-31
- fix: handle missing pit stop data in cached sessions


### 2024-04-01
- feat: implement live WebSocket broadcast for session data


### 2024-04-02
- fix: correct tyre compound mapping for 2022 season codes


### 2024-04-03
- test: add unit tests for lap time parser


### 2024-04-03
- chore: pin pandas version for dtype compatibility


### 2024-04-03
- feat: add pit stop detection and automatic lap exclusion


### 2024-04-05
- feat: add automatic reconnection for dropped clients


### 2024-04-18
- feat: implement DRS zone detection from car data channels


### 2024-04-20
- feat: add gear trace visualization alongside speed profile


### 2024-04-22
- fix: correct lap time parsing for sector 3 edge case


### 2024-04-23
- refactor: extract circuit map renderer to separate class


### 2024-04-24
- test: add WebSocket broadcast unit tests


### 2024-04-25
- fix: correct DRS detection for Monaco street circuit


### 2024-04-29
- perf: cache computed distance axis to avoid recomputation


### 2024-05-08
- feat: add multi-driver telemetry comparison overlay


### 2024-05-17
- feat: implement multi-client WebSocket fan-out server


### 2024-05-26
- fix: correct tyre compound mapping for 2022 season codes


### 2024-05-29
- fix: handle DNF laps in multi-driver comparison mode


### 2024-05-29
- chore: pin pandas version for dtype compatibility


### 2024-05-31
- test: add tests for telemetry alignment edge cases


### 2024-06-01
- feat: add compound strategy timeline for full race


### 2024-06-01
- feat: implement interpolated distance axis for alignment


### 2024-06-09
- refactor: extract circuit map renderer to separate class


### 2024-06-10
- refactor: rename ambiguous variables in lap parser module


### 2024-06-11
- refactor: extract telemetry loading into dedicated module


### 2024-06-30
- refactor: move all plotting functions to visualizer module


### 2024-07-01
- feat: add CSV export for aligned telemetry channels


### 2024-07-02
- chore: update FastF1 dependency to 3.3.x


### 2024-07-03
- feat: implement session selection via interactive prompt


### 2024-07-04
- fix: correct time alignment when laps share same timestamp


### 2024-07-17
- style: format all source files with black


### 2024-07-23
- feat: implement DRS zone detection from car data channels


### 2024-07-24
- feat: implement driver pace heatmap by lap


### 2024-07-25
- perf: use numpy vectorisation in telemetry alignment


### 2024-07-31
- test: add regression test for DNF lap exclusion logic


### 2024-07-31
- fix: handle FastF1 API rate limit with backoff


### 2024-08-02
- docs: add circuit map colour legend documentation


### 2024-08-03
- feat: add CSV export for aligned telemetry channels


### 2024-08-07
- feat: implement multi-client WebSocket fan-out server


### 2024-08-08
- feat: add gap-to-leader streaming in milliseconds


### 2024-08-08
- refactor: rename ambiguous variables in lap parser module


### 2024-08-19
- fix: fix incorrect lap count when VSC period is active


### 2024-08-19
- feat: implement DRS zone detection from car data channels


### 2024-08-19
- feat: implement synthetic lap data fallback for CI


### 2024-08-22
- fix: handle missing pit stop data in cached sessions


### 2024-08-22
- docs: document WebSocket message schema in docs/API.md


### 2024-08-26
- feat: add session selector for race qualifying and practice


### 2024-08-27
- fix: resolve crash when selected driver has zero valid laps


### 2024-08-27
- chore: add pre-commit hooks for black and ruff


### 2024-08-27
- refactor: extract telemetry loading into dedicated module


### 2024-08-29
- docs: update installation steps for Windows users


### 2024-08-30
- refactor: move all plotting functions to visualizer module


### 2024-09-03
- test: add integration test with cached 2023 session data


### 2024-09-03
- perf: cache computed distance axis to avoid recomputation


### 2024-09-05
- feat: implement lap telemetry parser for speed and throttle channels


### 2024-09-06
- chore: update FastF1 dependency to 3.3.x


### 2024-09-09
- perf: cache computed distance axis to avoid recomputation


### 2024-09-17
- fix: correct DRS detection for Monaco street circuit


### 2024-09-22
- perf: reduce peak memory in multi-driver comparison


### 2024-09-28
- fix: resolve crash when selected driver has zero valid laps


### 2024-09-29
- feat: implement lap telemetry parser for speed and throttle channels


### 2024-10-01
- feat: implement DRS zone detection from car data channels


### 2024-10-08
- feat: implement weather condition overlay on race charts


### 2024-10-18
- fix: correct sector boundary detection for specific circuits


### 2024-10-21
- docs: add circuit map colour legend documentation


### 2024-10-29
- feat: implement session selection via interactive prompt


### 2024-11-05
- feat: implement brake pressure overlay on lap comparison


### 2024-11-07
- feat: add multi-driver telemetry comparison overlay


### 2024-11-11
- feat: implement brake pressure overlay on lap comparison


### 2024-11-13
- feat: implement batch circuit map export for all drivers


### 2024-11-19
- feat: add automatic reconnection for dropped clients


### 2024-11-27
- feat: add rich terminal UI with live leaderboard display


### 2024-11-28
- fix: handle FastF1 API rate limit with backoff


### 2024-12-02
- fix: handle missing pit stop data in cached sessions


### 2024-12-06
- fix: handle FastF1 API rate limit with backoff


### 2024-12-06
- fix: correct sector boundary detection for specific circuits


### 2024-12-13
- fix: handle missing pit stop data in cached sessions


### 2024-12-14
- docs: update architecture diagram in docs/architecture.md


### 2024-12-19
- refactor: separate visualization from data processing logic


### 2024-12-20
- fix: fix matplotlib display on headless CI environments


### 2024-12-26
- perf: cache computed distance axis to avoid recomputation


### 2025-01-02
- style: normalise import ordering with isort


### 2025-01-07
- fix: correct tyre compound mapping for 2022 season codes


### 2025-01-12
- refactor: consolidate session loading into utility class


### 2025-01-15
- fix: handle missing telemetry for early 2022 season races


### 2025-01-19
- docs: document WebSocket message schema in docs/API.md


### 2025-01-20
- feat: add compound strategy timeline for full race


### 2025-02-03
- feat: add pit stop detection and automatic lap exclusion


### 2025-02-05
- feat: implement weather condition overlay on race charts


