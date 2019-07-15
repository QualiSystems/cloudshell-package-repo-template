# CloudShell package repo template

Use this template for creating a new package for the Shells.

## tox.ini
- set package-name var regarding your package
- set python version in envlist

## .travis.yml
- set python version regarding to tox.ini

## pyproject.toml
- set python version for black

## setup.py
- set name and description for the package
- set python version

## add git hook
run `pre-commit install`
