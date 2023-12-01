# Contributing to F1 Telemetry Visualizer

Thank you for your interest in contributing! Please follow the steps below to get your changes reviewed and merged.

---

## Workflow

1. **Fork** the repository to your own GitHub account.
2. **Create a branch** from `main` with a descriptive name:
   ```bash
   git checkout -b feature/my-new-feature
   ```
3. **Make your changes**, keeping commits focused and atomic.
4. **Commit** with a clear, present-tense message:
   ```bash
   git commit -m "Add speed trace export to PNG"
   ```
5. **Push** your branch to your fork:
   ```bash
   git push origin feature/my-new-feature
   ```
6. **Open a Pull Request** against the `main` branch of this repository. Fill in the PR template and link any relevant issues.

---

## Code Style

This project enforces consistent formatting and linting via:

- **[black](https://github.com/psf/black)** — opinionated code formatter. Run before committing:
  ```bash
  black .
  ```
- **[ruff](https://github.com/astral-sh/ruff)** — fast Python linter. Run before committing:
  ```bash
  ruff check .
  ```

Both tools are included in `requirements.txt`. A pre-commit configuration is recommended but not required.

---

## Tests

Tests live in the `tests/` directory and are run with **pytest**:

```bash
pytest
```

Please add or update tests for any logic you change. PRs that reduce test coverage without justification will be asked to include tests before merging.

---

## Questions

Open an issue or start a discussion if you are unsure about the direction of a change before investing time in implementation.
