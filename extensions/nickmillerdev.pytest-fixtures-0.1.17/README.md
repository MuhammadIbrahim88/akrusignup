# pytest-fixtures README

VSCode extension to provide intellisense for Pytest Fixtures. Inspired by [pytest-vscode](https://github.com/cameronmaske/pytest-vscode). Uses `pytest --fixtures` to get fixture information.

## Demo

![demo](https://github.com/nickjmiller/pytest-fixtures/raw/HEAD/demo.gif)

## Features

* Autocomplete suggestions for parameters of test functions where fixtures may be used. Includes docstrings. Context aware of different fixtures available for each file.
* Go To Definition support. Uses pytest output to determine location of fixture.

Will first check `"python.testing.pytestPath"` for pytest, then will fallback on `python -m pytest` with the selected interpreter.

## Requirements

* Python
* pytest


## Known Issues

* Does not support typing of fixture parameters.
* Python extension provides a self-referential definition of function parameters so there will be two definitions, see [here](https://github.com/microsoft/vscode-python/issues/18536)

## Release Notes

[Change Log](https://github.com/nickjmiller/pytest-fixtures/blob/HEAD/CHANGELOG.md)
