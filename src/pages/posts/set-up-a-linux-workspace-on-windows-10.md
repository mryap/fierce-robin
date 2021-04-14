---
title: Set-up a Linux workspace on Windows 10
subtitle: How I do it
date: 2021-04-14T11:57:28.607Z
thumb_img_path: /images/screenshot-2021-04-14-125854.png
template: post
---
<!--StartFragment-->

The [Windows Subsystem for Linux (WSL)](https://docs.microsoft.com/en-us/windows/wsl/about) is a way to run a full Linux environment on Windows machine, without having to install a virtual machine, such as Virtual Box, VM Ware, or Hyper-V.

I learn that enabling 'Turn Windows features on and off' and tick the box next to Windows Subsystem for Linux is the first step. It will not gives you the WSL 2.  I need to

> Download [the WSL2 Linux kernel update package for x64 machines](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi) and install it. 

After install, I have to run<!--StartFragment-->

`wsl --set-default-version 2` in any PowerShell window. 

<!--EndFragment-->

Once the system restarts, I'll open up Microsoft Store, search for Ubuntu and in the Apps section, here's Ubuntu 18 04. I'll click on it and download an Ubuntu environment that will run on top of the Windows Subsystem for Linux. 

<!--EndFragment-->

<!--EndFragment-->

<!--EndFragment-->

turn Windows features on and off.

<!--EndFragment-->

<!--EndFragment-->

<!--EndFragment-->

<!--StartFragment-->

First, I install Windows Subsystem for Linux and then we'll restart, and then we'll install the Ubuntu package from the Windows store. So, to get started, I'll search for turn Windows features on and off. In the window that pops up, I'll scroll down to the bottom and tick the box next to Windows Subsystem for Linux. Then I'll press OK. I need to restart my system now, so I'll do that.



<!--EndFragment-->