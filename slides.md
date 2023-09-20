---
marp: true
footer: 2023-09-23
header: Linux Party
paginate: true
---
# **Linux Party**

2023-09-23

FOCS Group

---

# What is Linux

Linux has just past its 32nd birthday. In many devices, including (almost all) web servers, Android smartphones, electric cars, and of course on Steam Decks, you can find Linux.

Linux is an operating system *kernel*. Kernel means "core; central part" in English. Linux on itself can only respond to hardware events; there are no ways to interact with the Linux kernel directly.

People bundle software (browsers, file managers, etc.) together with the Linux kernel to form a functional operating system. Many different people and companies bundle various software with Linux, each coming with their own configurations (wallpapers, theme, etc.) Various "flavors" of the Linux operating system, or *Linux distributions*, are thus created.

Today, we will help you to install a Linux distribution on your computer. You can choose Ubuntu, one of the most popular Linux distributions; or choose FOCS Debian, a Debian-based distribution which is developed by and for fellow JIers. Also you can choose other distributions.

---

# Linux and Linux Distributions

![h:550px](./choose%20your%20system.jpg)

Screenshot from LinusTechTips


---

# FOCS Debian

- Features a similar interface to Windows 10. Windows users will feel at home
- Developed from base system to avoid redundant software as in the official Debian images
- Aims to lower the time spent by students on installing software during labs
- Has the following software pre-installed:

<table style="display: block; margin: 0 auto;"><tr>
<td>
<img   height="100" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/c02ddb98-80e8-4d07-a80a-a68c84349761" >
</td>
<td>
<img  height="100" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/69f0b790-4c42-4b7e-b979-f4d6bf509e43">
</td>
<td>
<img  height="100" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/0d4d48e3-065a-46e4-88bf-0a92c6376004">
</td>
<td>
<img height="100" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/54ce2410-b9c4-48b2-b46e-1e0c6dd3728b">
</td>
<td>
<img  height="100" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/84f54de9-6904-4157-8647-880f234d61dc">
</td>
</tr></table> 

---
# Benefits of having a Linux system

- Survive 151, 280, 482 and other JI courses without having to worry about configuring your system
- More control of your computer; no disturbing desktop ads anymore, no worrying about Big Brother watching you ;)
- A bonus point on your resume that can help you find a job
- Most importantly...
- Linux is fun! Welcome to the world of FOSS, Free and Open Source Software!

---

# Ways to get a Linux system

- Use Windows Subsystem on Linux - WSL
- Use a virtual machine 
- Install a dual boot system
- Only use Linux on your computer

---
# Administering a Linux system

Linux is pretty much designed around a command-line shell. A _shell_ is a program that interacts with the operating system _kernel_: you issue commands via the shell, and the OS does it for you. In order to master Linux, some basic shell knowledge is necessary.

---
# Alternatives of common Windows tools
- Chrome, Edge, 360 Browser ... -> Firefox, Chromium
  - Install by the App Store provided by your distribution, or
  - Type in `sudo apt install firefox` or `sudo apt install chromium` in a terminal to install them (Debian and Ubuntu)

- Microsoft Office -> LibreOffice, WPS Office
  - It is likely that you have LibreOffice pre-installed on your system
  - You may download WPS Office from the Internet if you wish
- Your distribution likely provides you with a App Store. You may install apps there
- Chinese Input Method -> `ibus` (easier to configure, bundled with Ubuntu by default), `fcitx5` (more powerful and more features)

---

# Where can I find help and support

- First things first: Search on **Google** in **English**. Searching on Baidu won't return useful results in most cases :)
- Check your distro's Wiki. For example, Ubuntu Wiki is hosted at https://wiki.ubuntu.com
- Arch Linux Wiki often have know-how that you want. Check https://wiki.archlinux.org if you can't find help on your distro Wiki
- Join FOCS Mattermost! We are available at https://focs.ji.sjtu.edu.cn/mm at any time. You are always welcomed!
- You may also join a local Linux User Group. SJTU have its own Linux User Group; check https://sjtug.org for how to join them
