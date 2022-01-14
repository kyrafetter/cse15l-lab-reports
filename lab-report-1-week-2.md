# Lab 1: Remote Access and the File System

*January 13, 2022*

Welcome to my first tutorial! In this lesson we will learn the basics of connecting to a server via ssh, moving files between the client and server, practicing basic bash commands, and much more! 

**Note**: The following tutorial will be done using a Windows device as the model device. 

## Objectives
1. Download and install VScode
2. Remotely connecting via ssh
3. Learn basic bash commands
4. Moving files over ssh with srp
5. Setting up an ssh key
6. Optimizing remote running

## Procedure

> **1. Downloading and Installing VScode**
1. Navigate to the Visual Studio Code website ([click here](https://code.visualstudio.com/)) to download and install VScode on your device. Make sure the you select the correct version for your device. In this case, we select "Download for Windows": 
![Image](Screenshot%202022-01-13%20215708.png)

2. When installed, open VScode and you should get a window like this:
![Image](Screenshot%202022-01-13%20120515.png)

> **2. Remotely Connecting to a Server**
1. Install OpenSSH ([click here](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)). This program enables connection to a server via ssh.
2. Lok up your course-specific account for your UCSD course ([click here](https://sdacs.ucsd.edu/~icc/index.php)). Take note of the three letters specifying your account. **Note**: you may need to reset your password. To do so, click "Change your Passowrd". Make sure you indicate "no" for "Change my TritonLink Password". The change may not activate for 10-15 minutes. 
3. Open terminal in VScode (Terminal -> New Terminal)
4. Use the ssh command to connect to the server. Make sure to replace `zzz` with your account letters:
```
ssh cs15lwi22zzz@ieng6.ucsd.edu
```
5. Respond "yes" to the authenticity of host message in order to continute connecting.
6. Type your password (IT WON'T SHOW UP AS YOU TYPE) and push "Enter". Once you log in, your screen should look like this:
![Image](first_login.png)
7. **Note**: This indicates that you (the client) have logged into computer 201 (the server) of the ieng6 cluster. Yay!
> **3. Trying Some Commands**

**Note**: `~` represents your home/base directory
1. These are some useful bash commands to try:
    * `cd` -> change directory
    * `ls`  -> list items in working directory (excluding dotfiles)
    * `ls -lat` -> list items in working directory by date 
    * `ls -a` -> list **all** items in working directory (including dotfiles)
    * `pwd` -> print path to current working directory
    * `mkdir` -> create a new folder in working directory
    * `cp` -> cp a file into another file 
    * `cat` -> view the contents of specified file
2. To log out, either...
    * Ctrl-D
    * Use the `exit` command
* Here are some examples of the the commands above:

    *copying a file from a directory on another account to my home directory*
![Image](bash_command.png)

> **4. Moving Files with scp**

> **5. Setting an SSH Key**

> **6. Optimizing Remote Running**


