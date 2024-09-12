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


