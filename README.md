# Setting-up-a-Python-development-environment
# LINUX
### 1. To install Python in a Linux environment, install the appropriate packages for your distribution. For Debian and Ubuntu, these packages are python3, and python3-dev, and python3-venv.

##### Install these packages using the following commands:
sudo apt update 

sudo apt install python3 python3-dev python3-venv

or

sudo yum install python3 python3-dev python3-venv

### 2. You also need to install pip. While Debian and most other distributions include a python-pip package, we recommend that you install pip yourself to get the latest version:
wget https://bootstrap.pypa.io/get-pip.py

sudo python3 get-pip.py

### 3. After the installations are complete, verify that you have pip installed:
pip --version

--------------------------
## Use the venv command to create a virtual copy of the entire Python installation. This tutorial creates a virtual copy in a folder named venv, but you can specify any name for the folder.
venv is a tool that creates isolated Python environments. These isolated environments can have separate versions of Python packages, which allows you to isolate one project's dependencies from the dependencies of other projects. We recommend that you always use a per-project virtual environment when developing locally with Python.

### 1. Use the venv command to create a virtual copy of the entire Python installation. This tutorial creates a virtual copy in a folder named venv, but you can specify any name for the folder.
cd your-project

python3 -m venv venv

### 2. Set your shell to use the venv paths for Python by activating the virtual environment.
source venv/bin/activate

If you want to stop using the virtual environment and go back to your global Python, you can deactivate it:
deactivate
### 3. Now you can install packages without affecting other projects or your global Python installation:
pip install google-cloud-storage

### Make reference to the link for details (Include: MacOS, Windows, Linux)
https://cloud.google.com/python/setup#linux

# WINDOWS OS
https://docs.python.org/3/tutorial/venv.html

SET UP VIRTUAL ENVIRONMENT ON WINDOWS:

#python3 -m venv C:/myvenv
python -m venv C:/myvenv

#Start service
C:\myvenv\Scripts\activate.bat
