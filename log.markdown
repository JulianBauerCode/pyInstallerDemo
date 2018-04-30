#Literature:
https://pythonhosted.org/PyInstaller/operating-mode.html

# Make Executable for Linux

## Set up virtual environment
### Create virtual environment once
virtualenv -p python3.5 ~/pyInstallerDemo
### Active virtual environment
source ~/pyInstallerDemo/bin/active

## Create simple python program 
echo "print('Hello')" > hello.py

## Test the program
python3 hello.py

## Install pyInstaller 
pip install pyInstaller

## Use pyIstaller
pyinstaller hello.py

## Use results
PyInstaller creates two directories.
 + build
 + dist
The directory 'build' is only used during the process of building the other directory and can be deleted
Execute the program frozen by pyInstaller by executing
cd dist/hello/
./hello


#Make Executable on Ubuntu for Windows7

## Install wine
sudo apt-get install wine 

## Install python2
winetricks python installs 

## Installation of Python3.5 failed and suggests installing python3.
Following the installation process in the GUI is not possible after executing
wine msiexec /i python-3.4.4.amd64.msi  

Resigned installation of python3.x

Following the installation process in the GUI is not possible after executing

wine msiexec /i python-2.7.10.amd64.msi
fixme:msi:ControlEvent_SpawnWaitDialog Doing Nothing

Installing 32-bit version of wine and retry installation of python version may would succed


