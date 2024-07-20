# Documentation
This repo contains my personal setup for development.

## Table of Contents
1. [VSCode General Settings](#vscode)
1. [Python](#python)
1. [SQL](#sql)

## VSCode
For VSCode specific settings, there is a config file located at `.vscode/settings.json`. Generally, this file contains settings to correctly utilize any VSCode extensions as well as set up rulers to get a sense of character limits.

___

## Python
For formatting Python files, `isort` and `black` are used to autoformat.
### Linters/Formatters
- [isort](https://pycqa.github.io/isort/)
  - Sorts imports at the top of the .py file.
- [black](https://github.com/psf/black)
  - Autoformats python files
### Config
These extensions and libraries don't require much configuration apart from when the formatting should be executed. See 
[VSCode General Settings](#vscode) for the configuration.

___

## SQL
SQLFluff is used for linting and formatting SQL files with a large amount of configuration.
### Linters/Formatters
- [SQLFluff](https://github.com/sqlfluff/sqlfluff)
  - Lints/Formats SQL files
### Config
To configure the sqlfluff VSCode extension, see [VSCode General Settings](#vscode). This file mainly configures paths and when the linting/formatting should be executed.

To configure the style of the SQL code, a `.sqlfluff` file is provided.

___