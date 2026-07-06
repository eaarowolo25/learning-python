
[Real Python #1](https://realpython.com/effective-python-environment/)

## Shells
A shell is a program that provides a text based interface to you which you can use a command-line interface (CLI) to execute commands and see their output.

Different type of shells:
1. Unix Shells
2. Bourne Shell (sh)
	- first shell to incorporate environment variables, conditionals and loops.
3. Bourne-Again Shell (bash)
	- bash provides more data types like arrays
	- bash expands on sh with improved user-interaction features
4. Xonsh
5. CMD
6. PowerShell

## Terminal Emulators
The terminal was what early developers used. Today,  the terminal is where you access the shell.
They all have the same basic features:
- text colours for highlighting syntax
- scrolling for viewing earlier commands and outputs
- copy/paste
- tabs for running multiple programs at the same time

## Python Version Management
Sometimes you will need to run multiple versions of Python.

*pyenv*:
- pyenv is a tool for installing and managing multiple Python versions on MacOS
- Can manage local, global. and per project versions of python.

```
pyenv global 3.7.3
pyenv versions

pyenv local 3.7.3
pyenv versions

pyenv shell 3.7.3
pyenv versions

python --version
```


## [[Virtual Environment - Python|Virtual Environments]]
Is a way to save a projects installed packages and python version.
You just pass it a location to save the virtual environment

**venv**:
```
python -m venv {filepath}

#to activate it
source {path}/activate

#to deactivate
deactivate
```

**pyenv-virtualenv**:
```
#to create the environment
pyenv virtualenv 3.7.3 my-env

#activate virtual environment
pyenv activate my-env

#exit virtual environment
pyenv deactivate
```

## Package Management
[[pip - package management|**pip**]] (pip install packages) is the number 1 package management tool in Python. It automates the process of downloading packages and making python aware of it.

Install all the dependencies:
```
python -m pip install -r requirements.txt
```
