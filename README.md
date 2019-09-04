# CloudShell package repo template

[![Build status](https://travis-ci.org/QualiSystems/cloudshell-package-repo-template.svg?branch=dev)](https://travis-ci.org/QualiSystems/cloudshell-package-repo-template)
[![codecov](https://codecov.io/gh/QualiSystems/cloudshell-package-repo-template/branch/dev/graph/badge.svg)](https://codecov.io/gh/QualiSystems/cloudshell-package-repo-template)
[![PyPI version](https://badge.fury.io/py/cloudshell-package-repo-template.svg)](https://badge.fury.io/py/cloudshell-package-repo-template)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)

Use this template for creating a new package for the Shells.

## Description of services
### tox
It's a tool for running tests in multiple virtualenvs
To run all tests described in tox.ini just run `tox`
To run a particular env use `tox -e env_name`

### pre-commit
Run all code linters with a command `pre-commit run --all-files`  
Add git hook with command `pre-commit install`
- **isort** - sorting imports (config in tox.ini)
- **black** - reformat code to one style (config in pyproject.toml)
- **flake8** check code style (config in tox.ini), we use these plugins: flake8-docstring for checking docstrings; flake8-builtins for preventing using builtins as variable names; flake8-comprehensions to check list/dict comprehensions; flake8-print to prevent leaving prints in the code; flake8-eradicate to prevent leaving commented code

## Installation:

### tox.ini
- set package-name var regarding your package
- set python version in envlist

### .travis.yml
- set python version regarding tox.ini

### pyproject.toml
- set python version for black

### setup.py
- set name and description for the package
- set python version
