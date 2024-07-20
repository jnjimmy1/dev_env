# Welcome
This repo contains my personal setup for development with Python and SQL. See [docs](https://github.com/jnjimmy1/dev_env/blob/main/docs/main.md) for in-depth documentation.

## Overview
- Python
  - `isort` and `black` formatting
  - pre-commit

- SQL
  - `sqlfluff` linting and formatting
  - pre-commit

# Installation Steps
- Install VSCode and the following extensions
  - [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
  - [isort](https://marketplace.visualstudio.com/items?itemName=ms-python.isort)
  - [Black Formatter](https://marketplace.visualstudio.com/items?itemName=ms-python.black-formatter)
  - [sqlfluff](https://marketplace.visualstudio.com/items?itemName=dorzey.vscode-sqlfluff)
- Install conda or miniconda
  - On a terminal, navigate to the project directory:
    ```sh
    # Create conda environment using the provided environment.yml file
    conda env create -f -y environment.yml
    ```

# Running Dev Environment
- Open terminal and activate the conda env
    ```sh
    conda activate dev
    code . # Launch vscode at the current directory (or input path to the project directory)
    ```