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

Linux kernel has just past its 32nd birthday. In many devices, including web servers, smartphones, electric cars, and of course on Steam Decks, you can find Linux.

Linux is an operating system *kernel*. Kernel means "core; central part" in English. Linux on itself can only respond to hardware events; there are no ways to interact with the Linux kernel directly.

People bundle software (browsers, file managers, etc.) together with the Linux kernel to form a functional operating system. Many different people and companies bundle various software with Linux, each coming with their own configurations (wallpapers, theme, etc.) Various "flavors" of the Linux operating system, or *Linux distributions*, are thus created.

---

# Installing Linux

Today, we will help you to install a Linux distribution on your computer. You can choose Ubuntu, one of the most popular Linux distributions; or choose FOCS Debian, a Debian-based distribution which is developed by and for fellow JIers. Also you can choose other distributions.

---

# Linux and Linux Distributions

![h:550px](./choose%20your%20system.jpg)


---

# FOCS Debian

- Features a similar interface to Windows 10. Windows users will feel at home
- Developed from base system to avoid redundant software as in official Debian images
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

- Survive 151, 280, 281, 482 and other JI courses without having to worry about configuring your system
- More control of your computer; no disturbing desktop ads anymore, no worrying about Big Brother watching you ;)
- A bonus point on your resume that can help you find a job
- Most importantly... Linux is fun!

---

# Ways to get a Linux system

- Use Windows Subsystem for Linux - WSL
- Use a virtual machine 
- Install a dual boot system
- Only use Linux on your computer (advanced)

---
# Comparison of different installation methods

| Benefits\Method                                              | WSL                                            | Virtual Machine                         | Dual Boot   |
| ------------------------------------------------------------ | ---------------------------------------------- | --------------------------------------- | ----------- |
| Close integration with your current system (shared files, etc) | Yes                                            | No                                      | No          |
| Full-featured Linux                                          | No (sometimes GUI won't work)                  | Yes                                     | Yes         |
| Easy to install                                              | Yes                                            | Yes                                     | No          |
| Suitable for every-day use                                   | Yes                                            | No                                      | Yes         |
| Easy to customize and manage (change desktop wallpaper, tweak system parameters) | No                                             | Yes                                     | Yes         |
| Performance                                                  | High                                           | Low                                     | Best        |
| Hardware compatibility                                       | Adequate (sophisticated networking won't work) | Adequate (sometimes performance is low) | Good        |
| **Our recommendation**                                       | Just enough to survive                         | Recommended for newcomers               | Enthusiasts |

---
# Some FAQ after installing Linux

- Q: I want to install software under `D:\Program Files`. Where is it?
  - A: Linux have no `C:` or `D:`. Installing everything under the same disk is fine
  
- Q: Where are my documents, photos, films... stored?
  - A: You have a dedicated folder for all your personal files. If your username is `focs` then all your files lie under `/home/focs`. This is also the default startup folder of your file manager.
  
- Q: Where can I find software? 

  - A: In most cases you don't need to Baidu the software anymore. You have a *package manager* on your system that automatically grabs the software for you. See the following slides for details.




---
# Administering a Linux system

Linux is pretty much designed around a command-line *shell* (think of it as a far more powerful version of `cmd`).x In order to master Linux, some basic shell knowledge is necessary.

To launch a command-line shell, you may press **Ctrl**+**Alt**+**T** on Ubuntu and FOCS Debian; or you may find the application named `Terminal` in the application grid. macOS users may find themselves acquainted with the Terminal app.

![image-20230921152620642](terminal.png)

---
# Installing software

Many distros have an App Store bundled. Ubuntu have Snap Store; Fedora have GNOME Software Center; FOCS Debian have Discover. Installing software is just a one-click from there.

Some software (like C compilers, since they are command-line only) do require you to install them via the command line. You need to launch a terminal as described previously, and issue commands to your *package manager* to install them.

- Debian, Ubuntu: `sudo apt install software-name`

- Fedora, CentOS: `sudo yum install software-name`

- openSUSE: `sudo zypper in software-name`

- Arch Linux: `sudo pacman -Sy software-name`

Updating your system is also done by issuing the `upgrade` command to the package manager. There is no equivalent of Windows Update.

# Alternatives of common Windows tools

- Chrome, Edge, 360 Browser ... -> Firefox, Chromium

- Microsoft Office -> LibreOffice, WPS Office

- Chinese Input Method -> `ibus` (bundled with Ubuntu by default), `fcitx5` (more powerful and more features)

- QQ, WeChat -> QQ at https://im.qq.com/linuxqq; WeChat is more trivial, search Google for details

- Photoshop, Lightroom, Premiere Pro -> GIMP, darktable, Kdenlive

- MATLAB, Mathematica, and Vivado have native Linux versions

- Play games via Steam and Lutris (yes, you can play Genshin Impact)


---

# Where can I find help and support

- Check your distro's Wiki. For example, Ubuntu Wiki is hosted at https://wiki.ubuntu.com; Debian at https://wiki.debian.org
- Arch Linux Wiki often have the know-how that you want. Check https://wiki.archlinux.org if you can't find help on your distro Wiki
- Join FOCS Mattermost! We are available at https://focs.ji.sjtu.edu.cn/mm at any time. You are always welcomed!
- You may also join a local Linux User Group. SJTU has its own Linux User Group; check https://sjtug.org/contacts for how to join them

---

# Let's begin the Install Party!

Check the documentation of your preferred installation method.
