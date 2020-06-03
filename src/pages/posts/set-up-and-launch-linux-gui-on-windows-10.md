---
title: Set-up and launch Linux GUI on Windows 10
subtitle: No virtual machines or dual booting
date: 2020-06-01T08:27:42.454Z
thumb_img_path: /images/ezawltwxqaekqhl.jpg
template: post
---
No virtual machines or dual booting involve. Successfully set-up and launch the Desktop Graphical User Interface (GUI) or Linux DeskTop Environment 

![](/images/ezawltwxqaekqhl.jpg)

All this done under the hood in Windows 10 thanks to Windows Subsystem Linux (WSL). The set-up was run on WSL (also known as Bash on Windows).  WSL2 with native support for GUI apps was recently annouced during Microsoft Build 2020 - an annual event for software engineers and web developer that works primalry on WIndows, Microsoft Azure.

Under WSL, to have the GUI up and running, Xserver is require. 

These are the Linux command to install and run

```
sudo apt install lxde
```

```
export DISPLAY=:0
export LIBGL_ALWAYS_INDIRECT=1
```

```
startlxde
```

I heard about Windows Subsystem for Linux (WSL), and when I switched to Windows 10, I decided to explore it. I am not a full-stack developer and my area is in Data Analytics. Some cloud computing data analytics job process involve using Linxu environment and hence forth this is my motivation to pick-up Linux.

I used to install Virtual Machine (VM) to host Docker so I can work on some Data Science tutorial.

My interest with Linux piqued thanks to mucking around with Docker command. I have success with running Ubuntu on Virtual Machine on Windows 8. But not so with dual-booting. I tried and having 2 operating systems on a hard drive is a rabbit hole I regretted going down. (Another blog post on this some other time.)

The whole process from turning on WSL on Windows to installing all the essential Anaconda packages tooks me a good few 55 minutes. Your mileage might vary.