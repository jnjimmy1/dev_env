# dev_env
Boilerplate development environment

# Planned Tech Stack
- Python
  - isort and black formatters
  - pre-commit

- SQL
  - sqlfluff linter/formatter
  - pre-commit


```sh
conda create -n dev -y python,black,isort,ipykernel,pandas,numpy,boto3
conda activate dev
pip install sqlfluff

conda remove -n dev -y --all

conda env export --from-history > env.yml

conda env create -f environment.yml
```

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