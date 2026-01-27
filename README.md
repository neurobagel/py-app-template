<div align="center">

# py-app-template
Template for Neurobagel Python app, for use by Neurobagel maintainers.

[![Main branch checks status](https://img.shields.io/github/check-runs/neurobagel/py-app-template/main?style=flat-square&logo=github)](https://github.com/neurobagel/py-app-template/actions?query=branch:main)
[![Tests status](https://img.shields.io/github/actions/workflow/status/neurobagel/py-app-template/test.yaml?branch=main&style=flat-square&logo=github&label=tests)](https://github.com/neurobagel/py-app-template/actions/workflows/test.yaml)
[![Codecov](https://img.shields.io/codecov/c/github/neurobagel/py-app-template?token=Vn1do0lrCl&style=flat-square&logo=codecov&link=https%3A%2F%2Fcodecov.io%2Fgh%2Fneurobagel%2Fpy-app-template)](https://app.codecov.io/gh/neurobagel/py-app-template)
[![Python versions static](https://img.shields.io/badge/python-3.10--3.14-blue?style=flat-square&logo=python)](https://www.python.org)
[![License](https://img.shields.io/github/license/neurobagel/py-app-template?style=flat-square&color=purple&link=LICENSE)](LICENSE)

</div>

> [!WARNING]
> This template repo contains no application code directory and cannot be installed as-is.

## To finish creating a new repo from this template
- [Enable pre-commit ci](https://github.com/organizations/neurobagel/settings/installations/45014819) for the new repo
- Once you have created your main application code directory
  - in `pyproject.toml`, follow the `#TODO` comments to replace the app name placeholders
  - in `.github/workflows/test.yaml`, uncomment the steps to run the tests and upload coverage

### If the app is a CLI tool
- In `pyproject.toml`, uncomment the section for CLI-only config

### If releasing the package on PyPI
- In `pyproject.toml`, uncomment the section for packaging-only config
- In the [neurobagel/workflows sync config](https://github.com/neurobagel/workflows/blob/main/.github/sync.yml), add the new repo to the sync groups for auto-releasing Python projects on PyPI
- add PyPI badges for version and downloads, e.g.:
[![PyPI - Version](https://img.shields.io/pypi/v/bagel?style=flat-square&logo=pypi&link=https%3A%2F%2Fimg.shields.io%2Fpypi%2Fv%2Fbagel)](https://pypi.org/project/bagel/)
[![PyPI - Downloads](https://img.shields.io/pypi/dm/bagel?style=flat-square&logo=python&label=pypi%20downloads&link=https%3A%2F%2Fpypistats.org%2Fpackages%2Fbagel)](https://pypistats.org/packages/bagel)

## Provided in this template
- Project configuration via pyproject.toml
- pre-commit
- Code formatting and linting config:
  - flake8
  - black
  - isort
  - codespell
- pytest and code coverage with CodeCov integration
- `auto` configuration for automated releases
