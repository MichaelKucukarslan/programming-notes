### Trying to run the virtual environment did not go smoothly. I was having problems running the activate.bat file. 

Windows does not let you run scripts if you don’t have the right permissions. 

To allow the user to run scripts for the current process do this:

Open PowerShell as an administrator

#### Set proper permissions 
```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process
```

Note: This will allow you to run scripts while you are coding. Once you are done you don’t need to worry about removing permissions. `-Scope Process` means you can code while that in that command prompt. 

### Everything below will allow you to code forever but it is not safe to leave these permissions open. Use the code above and don’t worry about closing out permissions. 

  

This is a helpful site: [PowerShell Permissions](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.4)

## Important commands:

### Set the execution policy to undefined for the local machine

```bash
Set-ExecutionPolicy -ExecutionPolicy Undefined -Scope LocalMachine
```

### To be able to use scripts:
```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

### Be sure to turn this off when you are done programming. 
```bash
Set-ExecutionPolicy -ExecutionPolicy Undefined -Scope CurrentUser
```
; do this for everything. (LocalMachine, CurrentUser, Process, UserPolicy, MachinePolicy)