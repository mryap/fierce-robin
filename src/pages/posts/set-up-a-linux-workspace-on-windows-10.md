---
title: Set-up Linux workspace on Windows 10
subtitle: How I do it
date: 2021-04-14T11:57:28.607Z
thumb_img_path: /images/screenshot-2021-04-14-125854.png
template: post
---
<!--StartFragment-->

The [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/about) is a way to run a full Linux environment on Windows PC, without having to install a virtual machine, such as Virtual Box, VM Ware, or Hyper-V.

I learn that enabling 'Turn Windows features on and off' and tick the box next to Windows Subsystem for Linux is the first step. It will not gives you the WSL 2.  I need to download [the WSL2 Linux kernel update package ](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) and install it. 

![](/images/windows-features.png)

After install, I have to run in any PowerShell window<!--StartFragment-->

`wsl --set-default-version 2`  

<!--EndFragment-->

Once the system restarts,  open up Microsoft Store, search for Ubuntu in the Apps section. Look for Ubuntu 18.04 TLS., click on it and download an Ubuntu environment that will run on top of the Windows Subsystem for Linux. 

Python and Git comes together with Ubuntu 18.04.  TO verify, I run the following<!--StartFragment-->

```
python3 --version
```

<!--EndFragment-->

You can see that the set-up will occupy a place in your PC hard-drive as folder. This is to be expected. Fresh from the set-up in Ubuntu, type

```
# find the home folder

cd ~

# open up windows explorer for this folder

explorer.exe .
```



![](/images/screenshot-2021-04-14-132452.png "In the familiar Window Explorer, you should see those highlighted files and folders. ")

In the familiar Window Explorer, you should see those highlighted files and folders.   <!--StartFragment-->

You can now move files from Windows folders into this new networked folder. We’ll be able to access it from our WSL and interact with it as if it were still in the same Windows files. 

The way to create new folder in this Linxu environment, type (instead of point and click) 

```
mkdir helloWorld && cd helloWorld
echo 'print("hello from python on ubuntu on windows!")' >> hello.py
python3 hello.py 
```

<!--EndFragment-->

<!--StartFragment-->

In a remote Linux environment (this WSL Ubuntu is technically another machine without the User Interface, that just happens to be running locally on your computer)

<!--EndFragment-->

What Next? 

Network Isn’t [localhost](http://localhost) yet.  If you are building an application (NodeJS or SQL server), normally you would be able to check on your application right in your favourite browser using  `localhost` (<http://localhost:8000/>). In order for that to happen, check out [MS Accessing network applications](https://docs.microsoft.com/en-us/windows/wsl/compare-versions#accessing-network-applications) or install [Docker for Desktop](https://andrewlock.net/installing-docker-desktop-for-windows/#installing-docker-desktop-for-windows)

<!--EndFragment-->