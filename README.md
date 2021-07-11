# python3-dev-template

template repository for python3 development

## Create repository command memo

```shell
# git clone this repository
git clone https://github.com/neruo/python3-dev-template.git
cd ~/workspace/python3-dev-template

# setup poetry
poetry init -n
poetry env use python # create virtual environment
poetry add --dev flake8 black isort mypy
poetry shell # attach virtual environment

# setup vscode files: launch.json settings.json
git clone https://gist.github.com/278955c697d3788500e77521e57c47bb.git .vscode
rm -r .vscode/.git

# create start files: __init__.py run.py argument.py
git clone https://gist.github.com/c7830fa9d7aa62581b91da6d4a028ae3.git python3-dev-template
rm -r python3-dev-template/.git
```

## Usage

```shell
# setup poetry
poetry env use python # create virtual environment
poetry install # install packages
poetry shell # attach virtual environment
```