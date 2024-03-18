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


