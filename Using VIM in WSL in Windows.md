### In an Admin privileged CMD:

#### Try to Install WSL:  
```bash
wsl --install
```

#### Restart the computer.

### If you got an error about virtualization:
##### Enable virtualization on Windows
Control Panel > Programs > Turn Windows Features on or off > Hyper-V (Enable it)
Notes:[Enable virtualization on Windows](https://www.itechguides.com/how-to-enable-virtualization-in-windows-10/#Option_3_Enable_Virtualization_with_PowerShell)

You may need to allow for virtualization in the BIOS

#### Restart the computer.

### Try again:
```bash
wsl --install
```

### This will now install ubuntu Linux as a VM

#### If you want a different version you must specify a name

```bash
wsl --install -d <Distribution Name>
```

#### For the first install you will need to setup your user like any other Linux install. 

##### Some quick commands

| CMD                  | Info                |
| -------------------- | ------------------- |
| wsl                  | Starts the Linux VM |
| wsl --list           | Shows VM            |
| wsl --list --verbose | Shows more info     |
| wsl --shutdown       | Shuts down VM       |
Additional resources:
[Install wsl](https://learn.microsoft.com/en-us/windows/wsl/install)

  
#### One gotcha! Cmder doesn’t have select text with keyboard enabled by default. 

To do that got to settings in: 

`Keys & Macros > Mark/Copy > Select text with keyboard > Start selection with Shift + Arrow (Enable)`

### Setting up GIT in the new terminal
Since it is a new terminal in a new environment git will need to be configured. 

#### First check to see if git is installed. It should be but just check.

```bash
sudo apt-get install git
```
Any value for the version means it is installed.

#### Next setup your name and email.
```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@domain.com"
```
Resource:
[wsl-git](https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-git)

### Using VIM

Enter into the VM

```bash
wsl # This starts the VM
```

You can now cd into any folder on the computer like normal. 
```bash
vim <filename> # opens the file, if no file exists it creates the file
```
Additional Resources:
[Vim](https://vim.rtorr.com/)
**Good luck with vim!**

### Getting VIM to use auto complete:

This is going to take a while. 
Follow these steps to setup VIM version 9.0.0:

[install-latest-vim-ubuntu](https://itsfoss.com/install-latest-vim-ubuntu/)

Install Nodes JS version 
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.4/install.sh | bash
```
  
#### Restart the Linux terminal
```bash
nvm ls-remote
nvm install --lts
node -v
```
Your version should now be v20.16.0 or higher

Follow the steps here to setup plugins:
[vim-auto-complete](https://linuxhandbook.com/vim-auto-complete/)