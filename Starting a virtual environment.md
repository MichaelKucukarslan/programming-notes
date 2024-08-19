## For Windows:

You first need to start an execution policy that will allow you to start an environment. 
Use: 

```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
```

More Info: [Running Scripts in Windows 10](https://docs.google.com/document/u/1/d/1F7Lpxx5rR8hs4g8l0qAd7dM6wWGzoTXKtiEt7imMbLI/edit), [[Running a .bat script in Windows 10]]

### The start the environment:

```bash
env/Scripts/activate.ps1
```

More Info: [Creating a Virtual Environment](https://docs.google.com/document/u/1/d/1bC7bUVYHon8MzWOpJib8KzgP5a-QFwfHhiuHcBOKf1o/edit)

Together:

```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
env/Scripts/activate.ps1
```
  
## For Mac:

```bash
source env/bin/activate
```

More Info: [Creating a Virtual Environment](https://docs.google.com/document/u/1/d/1bC7bUVYHon8MzWOpJib8KzgP5a-QFwfHhiuHcBOKf1o/edit)