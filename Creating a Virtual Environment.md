## Create a project directory
```bash
mkdir <dir name>
cd <dir name>
```


### Create a new file
```bash
echo “Text to add” > <file name> ;creating it like this makes it UTF-16 and gives errors. Find the correct way
code -r <file name> ; opens the file in the same VSCode window
```
  

Note: <ctrl + ` > toggles the terminal

  

### Check for packages
```bash
pip freeze; shows you what packages are installed on the environment
```

  

### Create an include file for all the things for need to install on you virtual environment
```bash
pip freeze > requirements.txt
```
### Install requirements from that file
```bash
> pip install -r requirements.txt; Use this to install the requirments.txt
```
  
  

### Create a virtual environment
```bash
python -m venv <Name of environment> ; use env for the name
```
  

### To activate the environment
```bash
source env/bin/activate  ;for mac
env/Scripts/activate.ps1 ; for windows, note problem below
```
  

### Problem that arose:

Trying to run the virtual environment did not go smoothly. I was having problems running the activate.bat file. Look at this for Windows 10

[Running Scrpits in Windows 10](https://docs.google.com/document/d/1F7Lpxx5rR8hs4g8l0qAd7dM6wWGzoTXKtiEt7imMbLI/edit)

  

pip freeze ; should not have anything installed now


Running into a problem with pip :

[https://pip.pypa.io/en/stable/installation/](https://pip.pypa.io/en/stable/installation/) 

  

Using pip to install the requirements.txt:

[https://note.nkmk.me/en/python-pip-install-requirements/](https://note.nkmk.me/en/python-pip-install-requirements/)