---
title: Set-up and launch Linux GUI on Windows 10
subtitle: No virtual machines or dual booting
date: 2020-06-01T08:27:42.454Z
thumb_img_path: /images/ezawltwxqaekqhl.jpg
template: post
---
No virtual machines or dual booting. Successfully set-up and launch the Desktop Graphical User Interface (GUI).

![](/images/ezawltwxqaekqhl.jpg)

All this done under the hood in Windows 10 thanks to Windows Subsystem Linux (WSL) The set-up was run on WSL. WSL2 recently annouced om Microsoft Buld 2020 has support for GUI apps. 

To have the GUI up and running, Xserver is require. 

These are the Linux command

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