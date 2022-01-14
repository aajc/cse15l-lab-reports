# Lab Report 1
---
# VScode Installation
![Image](vscode.png)  

![Image](install.png)
* To start off this tutorial you need to [download VScode](https://code.visualstudio.com/), and it is an Integrated Development Environment where one can edit code.
* Simply click on download to download the application or the dropdown depending on your operating sytem.
* Then, run the installer and follow the instructions to fully install it on your computer.
# Remotely Connecting (SSH)
![Image](winSSH.png)
![Image](ssh.png)
* You will first need to [reset the password for your course account](https://sdacs.ucsd.edu/~icc/index.php) in the link above before anything else to enable your account in order to ssh.
* If you are on Windows you will need to follow [this tutorial](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse) which tells you to install two programs called open ssh client and server.
* Next you will want to remotely connect to the server, a remote computer.
* Enter the command ssh followed by (Your username)@(Hostname).
* Notice that you may be prompted about authenticity when connecting for the first time and you should enter yes.
# Running Some Commands
![Image](commands.png)
* The next order of business is running commands or instructions for the computer.
* As you can see in the image some starter commands include ls or list, cat or concatenate, cd or change directory, and exit to logout.
* Commands are ran by typing in the keyword sometimes followed by an argument separated by a space.
# Moving Files (scp)
![Image](scp.png)
* If you want to move files from your computer, the client, to the server you can use the scp command or secure copy.
* If you do not have ssh keys you will need to enter your password for your course account.
* The command is scp (local file) (Your username)@(Hostname):(desired directory location).
# SSH Keys
![Image](key.png)
![Image](mkdir.png)
![Image](sshkey.png)
* To get SSH keys you first need to run the ssh-keygen command which will generate two files, one for the client and one for the server designated as public, server, and private, client.
* Then you fill out the prompts and observe: where to store the public and private keys which are files (The overwrite prompt is there because I have already done this so it can be ignored), a passphrase for the keys, and then notice the information generated for your keys.
* To complete the process you need to ssh into your account, make an ssh directory for the public key, and logout to your local computer to scp the public key onto the server which will complete the process as the private key is only needed by the client.
# Becoming Efficient in the Remote Environment
![Image](mult.png)
![Image](exampleCommand.png)
* There are a myriad of tricks to optimize your remote running but a good start is using some basic ideas.
* These tricks include seperating commands with a ; on one line to do multiple commands in one go, you can couple this with attaching arguments to the ssh command, using keyboard shortcuts such as tab to finish arguments for you, and having an ssh key so you do not need to enter your password everytime you ssh or scp.
* An implementation of this would be to make coding java on a server a lot easier by on the same line sshing into the server and as the argument in "" you put javac file; java file; and cat file which would compile, run, and show the contents of the file in one command before returning to the local computer.
