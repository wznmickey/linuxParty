---
marp: true
---
# **Linux Party**

2023-09-23

FOCS Group

---

# What is Linux

Linux kernel has just past its 32nd birthday.[^1] In many devices including web servers, desktop computers and mobile devices, you can find Linux kernel.

Linux kernel is not easy to manage, so people create and add many components and release various distributions.

Today, we will help you to install a Linux distribution on your computer. You can choose Ubuntu, one of popular Linux distributions, or a Debian based distribution which is developed to be used for JI courses. Also you can choose other distributions.

---

# Linux and Its Distributions

![img_v2_3b252368-3113-48ff-bc60-0b8173a994eg](https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/08978295-2f54-4b81-a447-498db65b899d)

---

# FOCS Debian

- Has similar interface to Windows 10
- Developed from base system to avoid redundant software as in the official Debian images
- Aims to lower the time spent by students on installing software during labs
- Has the following software pre-installed:
<img align="center" width="100" height="100" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/c02ddb98-80e8-4d07-a80a-a68c84349761">
<img align="center" width="205" height="105" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/69f0b790-4c42-4b7e-b979-f4d6bf509e43">
<img align="center" width="211" height="125" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/0d4d48e3-065a-46e4-88bf-0a92c6376004">
<img align="center" width="284" height="125" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/54ce2410-b9c4-48b2-b46e-1e0c6dd3728b">
<img align="center" width="175" height="140" src="https://github.com/Bunyod-Suvonov/linuxParty/assets/109164894/84f54de9-6904-4157-8647-880f234d61dc">

---
# Ways to get a Linux system

- Use WSL
- Use virtual machine 
- Install a dual boot system
- Only use Linux

---
## Use WSL

If you use windows, it is the easiest way for you to have a Linux environment.
1. start Powershell in administer mode.
2. Type `wsl --install`.
3. Wait and then reboot.

https://learn.microsoft.com/en-gb/windows/wsl/install

If your windows version is old, please follow https://learn.microsoft.com/en-gb/windows/wsl/install-manual

---
## Use virtual machine 
You may choose VirtualBox or VMware.

https://software.sjtu.edu.cn/List/VirtualBox/virtualbox

1. Get the image (an `.iso` file) from the net.
2. Download and install the virtual machine software you want to use.
3. In the software, choose to create a virtual machine.
4. Choose the iso file you get.
5. Follow the instructions.
---
## Install a dual boot system

Be careful! Your data may be lost. **Make a backup** before you do the following steps.

1. Have a free disk partition. Have a USB disk.
2. Get the image (an `.iso` file) from the net.
3. Use tools like [rufus](https://rufus.ie/en/) to burn the iso into your USB disk.
4. Search online how to enter bios or uefi(different laptops require different key.) 
5. shutdown and then boot and enter bios or uefi.
6. Enable start from USB. Choose your USB disk to boot. Disable Secure Boot.
7. Boot and follow the setup steps.

When you choose the disk, be sure to check whether it is your **prepared free disk**.

---
## Only use Linux

The same as dual boot system. The only difference is to choose to install on your current system disk. 

*Your current system will **disappear**. All the data on your system disk will be **deleted**.*

---

# Setup your system

If you use WSL, your system will be setup by windows. You do not need to do anything.

Follow the instructions on the screen.

Here are some remainders.
1. Choose English. Do not use Chinese. It may cause many issues.
2. When choose the disk, be ***careful*** if you are not using virtual machine. It is recommend to have one partition for `/` and one partition for `/home/{yourname}` because you may have serval times erasing the system and reinstalling the system. 
---
# Start to use

1. Start Terminal.
2. Type `apt update` (apt is the package manager for debian-based systems. Yes, ubuntu is debian-based system.)
3. Install git, compiles and other tools you want to use by `apt install <name>`.

---
# Well known tools you could use in Linux
- Chrome, Edge, 360 Browser ... -> Firefox
- Microsoft Office -> Libre office, WPS(not opensource)
- App store -> apt (and many UI store integrated with apt)
- Chinese Input tools -> Sogou Pinyin(not opensource), Rime

[^1]: https://www.phoronix.com/news/Linux-6.6-rc2-Released
