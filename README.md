# Custom badook AI GitHub Actions
This repository contains custom GitHub actions required for badook AI CI/CD pipelines.

## Contributing
This repository uses [`pre-commit`](https://pre-commit.com/) for checking files committed to the repository. Install `pre-commit` by following the [installation guide](https://pre-commit.com/#install).

Locally install the pre-commit hook by executing `pre-commit install` in your repo folder.

## Included Actions

### Cached Install Poetry
This action installs [Poetry](https://python-poetry.org/) in a cached manner, as well as optionally installing [poetry-dynamic-versioning](https://github.com/mtkennerly/poetry-dynamic-versioning). It assumes that Python is already installed on the runner.

Internally, the actions uses the following 3rd-party actions:
* [snok/install-poetry](https://github.com/snok/install-poetry)

### Cached Poetry Install Dependencies
This action executes `poetry install` in a cached manner. It caches the created virtual environment for future use.
