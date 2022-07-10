# Python Virtual Environment

## _Install the virtualenv tool using your package manager_

Install the virtualenv tool using your package manager:

```sh
sudo apt install virtualenv
```

Create a `python-environments` directory in your user’s home directory and navigate to it:

```sh
mkdir ~/python-environments && cd ~/python-environments
```

Create a Python virtual environment. By default, virtualenv attempts to use the Python 2.5 interpreter to create a new environment. You can use the --python option to tell virtualenv to use your system’s Python interpreter. Replace env with the name you would like to assign to your virtual environment:

```sh
virtualenv env

```

The command creates a new directory with the name you assigned to your virtual environment. This directory contains all of the isolated files, packages, modules, and executables that is used by your new environment.

Validate that your environment is installed with the version of Python that you expect:

```sh
ls env/lib
```

You should see your env environments Python version:

```sh
python3.x.x
```

## _Activate Your Virtual Environment_

Activate the newly created virtual environment:

```sh
source env/bin/activate
```

The name of the working environment appears in parentheses after it’s created.

```sh
(env) example_user@hostname:~/python-environments$
```

You can now begin installing Python packages and libraries that will remain isolated to your virtual environment.

## _Deactivate a Virtual Environment_

To deactivate an active virtual environment, issue the following command:

```sh
deactivate
```

Your virtual environment is deactivated and you should no longer see its name listed next to your command line’s prompt

```sh
example_user@hostname:~/python-environments$
```
