---
title: Set-up and launch Linux GUI on Windows 10
subtitle: No virtual machines or dual booting
date: 2020-06-01T08:27:42.454Z
thumb_img_path: /images/ezawltwxqaekqhl.jpg
template: post
---
No virtual machines or dual booting involve. Successfully set-up and launch the Desktop Graphical User Interface (GUI) or Linux DeskTop Environment 

![](/images/ezawltwxqaekqhl.jpg)

All this done under the hood in Windows 10 thanks to Windows Subsystem Linux (WSL). The set-up was run on WSL. WSL2 with native support for GUI apps was recently annouced during Microsoft Build 2020 - an annual event for software engineers and web developer that works primalry on WIndows, Microsoft Azure.

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