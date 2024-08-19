You will first need to install PIP globally. After the global install you well need to upgrade it on all virtual environments.
### Open PowerShell as Admin
```bash
Start-Process powershell -Verb runAs
```

### Upgrade PIP Globally
```bash
python -m pip install --upgrade pip
```

### Installing on a virtual environment
#### Start the virtual environment
```bash
.\venv\Scripts\Activate
```

#### Download get-pip.py

```bash
curl.exe -O https://bootstrap.pypa.io/get-pip.py
```

#### Run get-pip.py

```bash
python get-pip.py
```

#### Upgrade pip in the virtual environment

```bash
python -m pip install --upgrade pip
```
