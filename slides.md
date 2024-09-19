---
marp: true
paginate: true
---
# **Linux Party**

2024-05-26

FOCS Team


---

# What is Linux

In many devices, including web servers, smartphones, electric cars, and of course on Steam Decks, you can find Linux.

Linux kernel itself does not support many functions, so people bundle software (browsers, file managers, etc.) together with the Linux kernel to form a functional operating system. Many different people and companies bundle various software with Linux, each coming with their own configurations (wallpapers, theme, etc.) Various "flavors" of the Linux operating system, or *Linux distributions*, are thus created.

---
# Installing Linux

Today, we will help you to install a Linux distribution on your computer. You can choose Ubuntu or Debian, two of the most popular Linux distributions; Also you can choose other distributions.

### Notes for macOS users

If you purchased your Mac after 2020, it is highly likely that your Mac features an Apple silicon processor. Apple Silicon processors can't run the software required by some JI courses, including Vivado and Solidworks. You are **highly recommended** to prepare a Windows computer (or other x86 based computer) as a backup. 

---

# Linux and Linux Distributions

![h:480px](https://github.com/wznmickey/linuxParty/assets/44784663/4c790df3-de1a-4674-babb-f2f75bce0fd9)

Screenshot from LinusTechTips

---

# Benefits of having a Linux system

- Survive 151, 280, 281, 482 and other JI courses without having to worry about configuring your system
- More control of your computer; no disturbing desktop ads anymore, no worrying about Big Brother watching you ;)
- A bonus point on your resume that can help you find a job
- Most importantly... Linux is fun!

---

# Ways to get a Linux system

- Use a virtual machine
- Use Windows Subsystem for Linux - WSL
- Install a dual boot system
- Only use Linux on your computer

---
# Comparison of different installation methods

| Benefits\Method                                              | WSL                                            | Virtual Machine                         | Dual Boot   |
| ------------------------------------------------------------ | ---------------------------------------------- | --------------------------------------- | ----------- |
| Close integration with your current system (shared files, etc) | Yes                                            | Part                                      | Part          |
| Full-featured Linux                                          | No (sometimes GUI won't work)                  | Yes                                     | Yes         |
| Easy to install                                              | Yes                                            | Yes                                     | No          |
| Suitable for every-day use                                   | Yes                                            | No                                      | Yes         |
| Performance                                                  | High                                           | Low                                     | Best        |

---

# Comparison of different installation methods
| Benefits\Method | WSL|Virtual Machine|Dual Boot|
|--|--|--|--|
| Easy to customize and manage (change desktop wallpaper, tweak system parameters) | No                                             | Yes                                     | Yes         |
| Hardware compatibility                                       | Adequate | Adequate | Good        |
| **Our recommendation**                                       | Just enough to survive                         | Recommended for newcomers               | Gaining more experience and fun |

---
# Where to get Linux installation images
USTC Mirror is a good starting point. It is located at https://mirrors.ustc.edu.cn
You can also use SJTU Mirror at https://mirrors.sjtug.sjtu.edu.cn 
Quick link: 
- ubuntu: https://mirror.sjtu.edu.cn/ubuntu-cdimage/releases/
- debian: https://mirror.sjtu.edu.cn/debian-cdimage/ports/current/
- deepin: https://mirror.sjtu.edu.cn/deepin-cd/releases/
![h:200px](./img/mirror.png)

---

# Some FAQ after installing Linux

- Q: I want to install software under `D:\Program Files`. Where is it?
  - A: Linux have no `C:` or `D:`. Different disks (partitions) are mounted at different path.

- Q: Where are my documents, photos, films... stored?
  - A: You have a dedicated folder for all your personal files. If your username is `focs` then all your files lie under `/home/focs`. This is also the default startup folder of your file manager.

- Q: Where can I find software? 

  - A: In most cases you don't need to search online for a long time to get the installer. You have a *package manager* on your system that automatically grabs the software for you. More details later.

---


# Administering a Linux system

Linux is pretty much designed around a command-line *shell* (think of it as a far more powerful version of `cmd`). In order to master Linux, some basic shell knowledge is necessary.

To launch a command-line shell, you may press **Ctrl**+**Alt**+**T** on Ubuntu and Debian; or you may find the application named `Terminal` in the application grid. macOS users may find themselves acquainted with the Terminal app.


---
# Package Manager and installing software

Most distribution have a built-in App Store based on some **package managers**. It is easy to use UI but some operations still need your CLI. Package managers automatically connect to a central software repository (you may need to change it to a mirror in China), download and install software for you. For Ubuntu and Debian, the package manager used is apt. Software installation is made easy and straightforward with the presence of package managers.

- To install software, run `sudo apt install <software-name>`
- To upgrade the system, run `sudo apt update && sudo apt upgrade`
- To remove installed software, run `sudo apt remove <software-name>`
- To search for something, run `apt search <software-name>`
  
There are also 2 new package managers called Snap and Flatpak. Their usage is similar to apt.

---

# Alternatives of common Windows softwares

MATLAB, Mathematica, Vivado, feishu, QQ, wechat and many other softwares officially support Linux now.

- Microsoft Office -> *LibreOffice*, WPS Office
- Chinese Input Method -> *`ibus`* (easier to configure), *`fcitx5`* (more powerful and more features)\
- MiKTeX, Overleaf TeX Editor -> *Texmaker*, or plugins in your editor
- Adobe Photoshop, Lightroom, etc. -> *GIMP*, *darktable* ...
- Solidworks -> *FreeCAD*, or check https://github.com/cryinkfly/SOLIDWORKS-for-Linux
- Games not support Linux -> *Lutris*

*softwares* in bold are open source.

---

# Where can I find help and support

- Use `man` and `--help` to get local help.
- Check your distro's Wiki. For example, Ubuntu Wiki is hosted at https://wiki.ubuntu.com; Debian at https://wiki.debian.org
- Arch Linux Wiki often have the know-how that you want. Check https://wiki.archlinux.org if you can't find help on your distro Wiki
- Search online and find solutions from forums and blogs.
- Join FOCS Mattermost! We are available at https://focs.ji.sjtu.edu.cn/mm/lobby/channels/linux at any time. You are always welcomed!
- You may also join a local Linux User Group. SJTU has its own Linux User Group; check https://sjtug.org/contacts for how to join them

---

# Let's begin the Install Party!

Check the documentation of your preferred installation method.
