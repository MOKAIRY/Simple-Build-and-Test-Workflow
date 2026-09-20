# Simple Build and Test Workflow

This project is a minimal Python example for a CI/CD build and test workflow. It includes a simple package setup and a basic pytest test to validate the project is working correctly.

## Project structure

- `setup.py` - package configuration
- `requirements.txt` - Python dependencies
- `tests/test_sample.py` - example test suite
- `.github/workflows/build-and-test.yml` - main CI workflow for build and test automation
- `.github/workflows/pull-request-status-checks.yml` - pull request validation checks
- `.github/workflows/storing-using-secrets.yml` - example workflow showing how to use GitHub secrets

## Requirements

Make sure Python is installed on your machine.

## Install dependencies

```bash
pip install -r requirements.txt
```

## Run tests

```bash
pytest
```

## Workflow files

This project includes three GitHub Actions workflow files in `.github/workflows/`:

- `build-and-test.yml` - runs the build and test pipeline
- `pull-request-status-checks.yml` - checks PR status and validation conditions
- `storing-using-secrets.yml` - demonstrates storing and using secrets in CI/CD jobs

## Example test

The sample test verifies the basic arithmetic check:

```python
def test_example():
    assert 1 + 1 == 2
```

This repository is intended as a simple starting point for learning automated builds and test pipelines.
