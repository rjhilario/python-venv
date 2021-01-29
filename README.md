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
1. Get the compressed archive file:
cd /tmp
wget https://www.python.org/ftp/python/3.7.9/Python-3.7.9.tgz

2. Unpack the that .tgz 
tar -xzvf Python-3.7.9.tgz

3. Change directory to extracted one
cd Python-3.7.9

4. Install dependencies need to compile the package
apt update
apt install -y 
