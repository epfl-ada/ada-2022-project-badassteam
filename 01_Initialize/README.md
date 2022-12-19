# spVPP
Velocity prediction program to beat the world sailing speed record

## First time setup (on windows) recommended

- Install Python 3.8.9 "https://www.python.org/downloads/release/python-389/"
- Install Git "https://git-scm.com/downloads"
- Install a code editor (recommend Visual Studio Code : "https://code.visualstudio.com/Download")
- Open a Command line or a terminal on VSC
- Create a folder in which you want to have the project files
- Clone the repository "git clone https://github.com/SP80VPP/VPP"
- Create a virtual environment for this code `python3 -m venv .\Python_venv_spVPP`
- Activate virtual environment `.\Python_venv_VPP\Scripts\activate`
- install pip-tools `pip install pip-tools`

## Install dev dependencies

- To use the script `pip-sync requirements.txt`
- To develop `pip-sync requirements_dev.txt`

## Add/remove dependencies

- edit the relevant requirement files (.in)
- compile the files
  ```
  pip-compile requirements.in
  pip-compile requirements_dev.in
  ```
# Github important point

- Create branch when creating new code
    - Allows for reviews
    - Make it easier for parallel developement
- Commit description with clear description (feat, refractor, fix)
- Always push your commit if the work of other depends on your code
- If multiple branch in parallel, rebase before merging

# Code quality

- Use linter and auto formater (pylint, black)
- Code scripts not notebooks
    - Possible to use script as a library in a notebooks for testing

## Visual studio code 
create a folder named ".vscode" and a file "settings.json"
with those parameters (customise the python path of your virtural env)
```
{
    "python.pythonPath": "c:\\Users\\YOUR_USERNAME\\YOUR_VIRTUAL_ENV_NAME\\Scripts\\python.exe",
    "jupyter.jupyterServerType": "local",
    "python.linting.enabled": true,
    "python.linting.pylintPath": "pylint",
    "editor.formatOnSave": true,
    "python.formatting.provider": "black",
    "python.linting.pylintEnabled": true,
    "python.globalModuleInstallation": true,
}
```
# Visual with Blender
- Download the last version of blender
- Copy the following script in a new script on blender
```
import subprocess
import sys
import os
python_exe = os.path.join(sys.prefix, 'bin', 'python.exe')
subprocess.call([python_exe, "-m", "ensurepip"])
subprocess.call([python_exe, "-m", "pip", "install", "--upgrade", "pip"])
subprocess.call([python_exe, "-m", "pip", "install", "pyzmq"])
```
- Launch the script with the "play" button on the top
- Close the blender file without saving
- Open the blender file [here](visualization/3D_visualization.blend)
- Launch the script with the "play" button on the top of the python script

# Viztracer
```
viztracer --log_multiprocess run_simulation.py
```

## Blender

- Install Blender
- Open the blender_simulation_live.py file
- In the Blender Python interpreter find the path to the python interpreter by typing ```import sys\nsys.exec_prefix```
- Open WindowsPowerShell in Administrator mode and go to the python interpreter folder
- Install pip with ```python -m ensurepip  ```
- Install ZeroMQ with ```python -m pip install pyzmq```
- Run the blender_simulation_live.py file
- Launch the simulation
