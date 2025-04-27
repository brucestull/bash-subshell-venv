# `TEMP-DIR` Notes

## Use `pipenv-env`'s `pipenv` to create a virtual environment in `TEMP-DIR`
```bash
flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ /home/flynntknapp/Programming/pipenv-env/venv/bin/pipenv install
Creating a virtualenv for this project
Pipfile: /home/flynntknapp/Programming/TEMP-DIR/Pipfile
Using /usr/bin/python3.12.3 to create virtualenv...
⠸ Creating virtual environment...created virtual environment CPython3.12.3.final.0-64 in 220ms
  creator CPython3Posix(dest=/home/flynntknapp/.local/share/virtualenvs/TEMP-DIR-z85xl9uM, clear=False,
no_vcs_ignore=False, global=False)
  seeder FromAppData(download=False, pip=bundle, via=copy, app_data_dir=/home/flynntknapp/.local/share/virtualenv)
    added seed packages: pip==25.0.1
  activators BashActivator,CShellActivator,FishActivator,NushellActivator,PowerShellActivator,PythonActivator

✔ Successfully created virtual environment!
Virtualenv location: /home/flynntknapp/.local/share/virtualenvs/TEMP-DIR-z85xl9uM
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.
Installing dependencies from Pipfile.lock (2110f5)...
flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Activate the virtual environment
```bash
flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ source ~/.local/share/virtualenvs/TEMP-DIR-z85xl9uM/bin/activate
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Check the Python packages installed in the `TEMP-DIR` virtual environment
```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ pip list
Package Version
------- -------
pip     25.0.1
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Use `pipenv-env`'s `pipenv` to install `pipenv` in the `TEMP-DIR` virtual environment

```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ /home/flynntknapp/Programming/pipenv-env/venv/bin/pipenv install pipenv
Courtesy Notice:
Pipenv found itself running within a virtual environment,  so it will automatically use that environment, instead of
creating its own for any project. You can set
PIPENV_IGNORE_VIRTUALENVS=1 to force pipenv to ignore that environment and create  its own instead.
You can set PIPENV_VERBOSITY=-1 to suppress this warning.
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.
Installing pipenv...
✔ Installation Succeeded
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.
Installing dependencies from Pipfile.lock (2110f5)...
All dependencies are now up-to-date!
Upgrading pipenv in  dependencies.
Building requirements...
Resolving dependencies...
✔ Success!
Building requirements...
Resolving dependencies...
✔ Success!
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.
Installing dependencies from Pipfile.lock (191bf3)...
All dependencies are now up-to-date!
Installing dependencies from Pipfile.lock (191bf3)...
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```
## Check the `Pipfile` of the `TEMP-DIR` virtual environment. It now includes `pipenv` as a dependency.
```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ cat Pipfile
[[source]]
url = "https://pypi.org/simple"
verify_ssl = true
name = "pypi"

[packages]
pipenv = "*"

[dev-packages]

[requires]
python_version = "3.12"
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Verify that `pipenv` is installed in the `TEMP-DIR` virtual environment

```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ pip list
Package      Version
------------ ---------
certifi      2025.4.26
distlib      0.3.9
filelock     3.18.0
packaging    25.0
pip          25.0.1
pipenv       2025.0.1
platformdirs 4.3.7
setuptools   79.0.1
virtualenv   20.30.0
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Verify that `pipenv` is installed in the `pipenv-env` virtual environment

```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ ~/Programming/pipenv-env/venv/bin/pip list
Package      Version
------------ ---------
certifi      2025.1.31
distlib      0.3.9
filelock     3.18.0
packaging    25.0
pip          24.0
pipenv       2025.0.1
platformdirs 4.3.7
setuptools   79.0.1
virtualenv   20.30.0
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Check location of `python` in the `TEMP-DIR` virtual environment

```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ which python
/home/flynntknapp/.local/share/virtualenvs/TEMP-DIR-z85xl9uM/bin/python
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Verify that `pipenv` is installed in the `TEMP-DIR` virtual environment

```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ pip list
Package      Version
------------ ---------
certifi      2025.4.26
distlib      0.3.9
filelock     3.18.0
packaging    25.0
pip          25.0.1
pipenv       2025.0.1
platformdirs 4.3.7
setuptools   79.0.1
virtualenv   20.30.0
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Install `django` in the `TEMP-DIR` virtual environment using `pipenv`

```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ pipenv install django
Courtesy Notice:
Pipenv found itself running within a virtual environment,  so it will automatically use that environment, instead of
creating its own for any project. You can set
PIPENV_IGNORE_VIRTUALENVS=1 to force pipenv to ignore that environment and create  its own instead.
You can set PIPENV_VERBOSITY=-1 to suppress this warning.
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.
Installing django...
✔ Installation Succeeded
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.
Installing dependencies from Pipfile.lock (191bf3)...
All dependencies are now up-to-date!
Upgrading django in  dependencies.
Building requirements...
Resolving dependencies...
✔ Success!
Building requirements...
Resolving dependencies...
✔ Success!
To activate this project's virtualenv, run pipenv shell.
Alternatively, run a command inside the virtualenv with pipenv run.
Installing dependencies from Pipfile.lock (7311d8)...
All dependencies are now up-to-date!
Installing dependencies from Pipfile.lock (7311d8)...
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Verify that `django` is installed in the `TEMP-DIR` virtual environment

```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ pip list
Package      Version
------------ ---------
asgiref      3.8.1
certifi      2025.4.26
distlib      0.3.9
Django       5.2
filelock     3.18.0
packaging    25.0
pip          25.0.1
pipenv       2025.0.1
platformdirs 4.3.7
setuptools   79.0.1
sqlparse     0.5.3
virtualenv   20.30.0
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

## Verify that `django` is installed in the `pipenv-env` virtual environment

```bash
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$ ~/Programming/pipenv-env/venv/bin/pip list
Package      Version
------------ ---------
certifi      2025.1.31
distlib      0.3.9
filelock     3.18.0
packaging    25.0
pip          24.0
pipenv       2025.0.1
platformdirs 4.3.7
setuptools   79.0.1
virtualenv   20.30.0
(TEMP-DIR) flynntknapp@DELL-DESKTOP:~/Programming/TEMP-DIR$
```

# bash-subshell-venv
