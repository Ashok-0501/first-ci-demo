# First CI Pipeline Using GitHub Actions

A small Python project demonstrating Continuous Integration (CI) with GitHub Actions.

## Project files

- `result_logic.py` — returns PASS when internal marks are at least 40 and attendance is at least 75; otherwise returns FAIL.
- `test_result_logic.py` — contains three automated unit tests.
- `.github/workflows/ci.yml` — runs the tests on pushes and pull requests targeting `main`, and supports manual workflow dispatch.

## Run locally

```bash
python -m unittest discover -v
```

GitHub Actions checks out the repository, sets up Python 3.11 on a GitHub-hosted Ubuntu runner, and runs the same tests automatically.
