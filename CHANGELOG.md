## v2.0.0 (2026-03-28)

### BREAKING CHANGE

- This separates language-specific dependency pinning
  from linter installation, configuration, and execution.

### Bug Fixes

- **python-build**: preserve the directory structure of build artifacts
- update the default Python version to 3.13
- mitigate supply chain attacks by pinning actions to commit objects

### New Features

- **pre-commit**: run linters from a dedicated common workflow

## v1.0.0 (2026-03-20)

### Bug Fixes

- mark required inputs and their default values
- **cz-bump**: correct the output release tag

### New Features

- control the generation and naming of changelog fragments
- define common Python CI workflows
