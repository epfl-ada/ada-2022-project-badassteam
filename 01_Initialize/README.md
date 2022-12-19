# Notebook bADAssteam

## First time setup (on windows) recommended

- Install Python 3.10.8 "https://www.python.org/downloads/release/python-3108/"
- Install Git "https://git-scm.com/downloads"
- Install a code editor (recommend Visual Studio Code : "https://code.visualstudio.com/Download")
- Install Anaconda "https://docs.anaconda.com/anaconda/install/"
- Open a Command line or a terminal on VSC
- Create a folder in which you want to have the project files
- Clone the repository "git clone https://github.com/epfl-ada/ada-2022-project-badassteam"
- Create a virtual environment for this code `conda create --prefix ADA_3.10 python=3.10`
- Activate virtual environment `conda activate ADA_3.10`
- install pip-tools `pip install pip-tools`

## Install dependencies to set environment

- Install all the predifined libraries `pip-sync requirements.txt`
- Install the NLP model `python -m spacy download en_core_web_sm`
- Install the NLP model `python -m spacy download en_core_web_lg`
- Install `coreferee` in english with `python -m coreferee install en`

## Add/remove dependencies

- edit the relevant requirement files (.in)
- compile the files
  ```
  pip-compile requirements.in
  ```
