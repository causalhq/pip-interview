# Causal Python Interview

## Cloning

:warning: the repo must be named as 'pip' when cloning for everything to work correctly :warning:

```
git clone git@github.com:causalhq/pip-interview.git pip
```

## Setup

Instructions geared for unix/mac using bash.

For windows see: https://pip.pypa.io/en/latest/development/getting-started/#get-the-source-code

### In home directory

```
brew install python@3.10
alias python=python3.10

python -m venv .venv
source .venv/bin/activate
python -m pip install nox
```

### In the repo

```
python -m pip install -e .
python -m pip --version
```

### Make sure this runs and passes

```
nox -s test-3.10 -- tests/unit/test_packaging.py
```
