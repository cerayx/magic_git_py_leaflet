#Getting started with the tutorial
##Downloading the project and Configuring Python
Before starting this section, you should have Python 3.4 and Git installed for 
your platform. If they are not installed, go back to the [Install Instructions](../README.md) 
before continuing.

###Cloning the repository
Open the terminal/command line application for your operating system (cmd.exe 
on Windows, Terminal on Mac OSX, varies on Linux). Use the `git clone` command 
to fetch the contents of this repository, which downloads a local copy to your 
machine:
```bash
git clone https://github.com/egoddard/magic_git_py_leaflet.git
```

###Move into the directory containing the tutorial
####Linux/OSX:
```bash
cd magic_git_py_leaflet/tutorial
```
####Windows:
```bash
cd magic_git_py_leaflet\tutorial
```

###Create a Python Virtual Environment
Virtual Environments keep your main Python installation from becoming 
cluttered with many packages, some of which could cause conflicts (some  
packages require specific versions of libraries to run). Virtual Environments 
also make it easy for you or others to reproduce the workspace, since all of the 
required libraries are stored in a text file and can be installed with a single 
command.

Create the virtual environment with:
####OSX
```bash
pyvenv venv
```
####Linux
If you are using a Debian or Ubuntu derivative, the OSX command above 
will not work for you. Unfortunately, Debian and Ubuntu (and Linux Mint) ship 
with a broken pyvenv. We can still use it, but we have to manually install pip 
(the tool that Python uses to install additional libraries):
```bash
#Debian/Ubuntu/Mint append the python version to the end of pyvenv
pyvenv-3.4 --without-pip venv
curl https://bootstrap.pypa.io/get-pip.py | venv/bin/python
```

Other distributions of Linux (Fedora, OpenSUSE, Arch, etc) should be able to 
use the OSX command above.

####Windows
Windows usually does not add the python interpreter to the environment path, 
so you have to use the full path name for the interpreter and the script:
```bash
c:\Python34\python c:\Python34\Tools\Scripts\pyvenv.py venv
```

The nice thing about virtual environments (especially in Windows) is that 
they temporarily add the python executable inside the `venv` folder to your 
path, which means that after activating the virtual environment (next step), 
simply executing `python` in the cmd.exe window will launch the python 
interpreter.

###Activate the virtual environment
####Linux/OSX
```bash
source venv/bin/activate
```
####Windows
On Windows, please use cmd.exe, not Powershell. Script execution is disabled 
by default in Powershell, which causes activation of the virtual environment 
to fail.
```batchfile
venv\Scripts\activate.bat
```

###Install the required Python libraries
Once the virtual environment is activated, python can be run from the command 
line by invoking `python` (all platforms). To install the 
python libraries we'll be using, run `pip install -r requirements.txt`.

###Deactivating the virtual environment
The Python virtual environment is only applied to the terminal in which it was 
activated. Closing the terminal will deactivate the virtual environment. If you want 
to use it again, run the activation command above for your platform.

To close the virtual environment without closing the terminal, use the 
`deactivate` command (all platforms).
