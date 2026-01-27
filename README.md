# py-app-template
Template for Neurobagel Python app, for use by Neurobagel maintainers.

## To finish creating a new repo from this template
- [Enable pre-commit ci](https://github.com/organizations/neurobagel/settings/installations/45014819) for the new repo
- Once you have created your main application code directory, in `pyproject.toml`, 
follow the `#TODO` comments to replace the app name placeholders

### If releasing the package on PyPI
- In `pyproject.toml`, uncomment the section for packaging-only config
- In the [neurobagel/workflows sync config](https://github.com/neurobagel/workflows/blob/main/.github/sync.yml), add the new repo to the sync groups for auto-releasing Python projects on PyPI

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
