---
title: Set-up Linux workspace on Windows 10
subtitle: No bloated virtual machines or dual-booting require
date: 2021-04-14T11:57:28.607Z
thumb_img_path: /images/screenshot-2021-04-14-125854.png
excerpt: No bloated virtual machines or dual-booting require
template: post
---
<!--StartFragment-->

The [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/about) is a way to run a full Linux environment on Windows PC, without having to install a virtual machine, such as Virtual Box, VM Ware, or Hyper-V.

I learn that enabling 'Turn Windows features on and off' and tick the box next to Windows Subsystem for Linux is the first step. It will not gives you the WSL 2.  You need to download [the WSL2 Linux kernel update package ](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) and install it. 

![](/images/windows-features.png)

After install, run in any PowerShell window 

`wsl --set-default-version 2`  

 Once the system restarts,  open up Microsoft Store, search for Ubuntu in the Apps section. Look for Ubuntu 18.04 TLS., click on it and download Ubuntu that will run on top of the Windows Subsystem for Linux. 

Python and Git comes together with Ubuntu 18.04.  TO verify, I run the following

```
python3 --version
```

You can see that the set-up will occupy a place in your PC hard-drive as folder. This is to be expected. Fresh from the set-up in Ubuntu, type

```
# find the home folder
cd ~
# open up windows explorer for this folder
explorer.exe .
```

![In Ubuntu environment, launch Windows Explorer and show the current directory in the WSL environment.](/images/screenshot-2021-04-24-080207.png "In the familiar Window Explorer, you should see those highlighted files and folders. ")

In the familiar Window Explorer, you should see those highlighted files and folders.   

You can now move files from Windows folders into this new networked folder. You’ll be able to access it from WSL and interact with it as if it were still in the same Windows files. 

To create new folder in this Linxu environment, type (instead of point and click) 

```
mkdir helloWorld && cd helloWorld
echo 'print("hello from python on ubuntu on windows!")' >> hello.py
python3 hello.py 
```



In a remote Linux environment (this WSL Ubuntu is technically another machine without the User Interface, that just happens to be running locally on your computer)

What Next? 

Network Isn’t localhost yet.  If you are building an application (NodeJS or SQL server), normally you would be able to check on your application right in your favourite browser using  `localhost` (<http://localhost:8000/>). In order for that to happen, check out [MS Accessing network applications](https://docs.microsoft.com/en-us/windows/wsl/compare-versions#accessing-network-applications) or install [Docker for Desktop](https://andrewlock.net/installing-docker-desktop-for-windows/#installing-docker-desktop-for-windows)

Alternatively, you can also set-up a [Linux Desktop environment ](https://www.testandoptimize.com/posts/set-up-and-launch-linux-gui-on-windows-10/)

Conclusion

[Windows Subsystem for Linux ](https://docs.microsoft.com/en-us/windows/wsl/about)(WSL) lets you run a Linux environment -- including command-line tools and applications -- directly on Windows, without the overhead of a traditional virtual machine or dualboot setup.  WSL helps web developers and those working with Bash and Linux-first tools (i.e. Ruby, Python) to use their toolchain on Windows. This ensure consistency between development and production environments.  When you install a version of Linux on Windows, you’re getting a full Linux environment. It's isolated from Windows- the UI is the terminal, and you can install tools, languages, and compilers into the Linux environment without modifying or disrupting your Windows installation.