# python-venv
Virtual Environment for Python 3.7.9


This repo is for setting up a Python Virtual Environment
and specifically for version 3.7.9


What is a Python Virtual Environment?
A virtual environment is a Python environment such that the Python interpreter, libraries and scripts installed into it are isolated from those installed in other virtual environments, and (by default) any libraries installed in a “system” Python, i.e., one which is installed as part of your operating system.

A virtual environment is a directory tree which contains Python executable files and other files which indicate that it is a virtual environment.

Common installation tools such as setuptools and pip work as expected with virtual environments. In other words, when a virtual environment is active, they install Python packages into the virtual environment without needing to be told to do so explicitly.

Full information can be found in official Python site:
https://docs.python.org/3/library/venv.html


Usage:
1. Get the compressed archive file:<br/>
`cd /tmp`<br/>
`wget https://www.python.org/ftp/python/3.7.9/Python-3.7.9.tgz`

2. Unpack the that <br/>
`tar -xzvf Python-3.7.9.tgz`

3. Change directory to extracted archive <br/>
`cd Python-3.7.9`

4. Install dependencies need to compile the package <br/>
`apt update`<br/>
`apt install -y build-essential openssl libssl-dev zlib1g-dev libffi-dev freetds-dev libbz2-dev libsqlite3-dev unixodbc-dev`

5. Compile with the recommended parameters below <br/>
`./configure --enable-optimizations --enable-loadable-sqlite-extensions && make altinstall`

6. Upgrade pip <br/>
`/usr/local/bin/python3.7 -m pip install --upgrade pip`

7. At this point you can initiate the virtual environment

```
python3.7 -m venv .venv37
source .venv37/bin/activate
python3 -m pip install --upgrade pip
python -V
pip -V
```

Please see sample requirements.txt file. It really depends on your project 
as to whatever package for pip you need. You need to install them so you
can properly run python codes/scripts.

`pip install -r requirements.txt`

This would largely depend on what kind of project you are working on.
