---
marp: true
---
# **Linux Party**

2023-09-23

FOCS Group

---

# What is Linux

Linux kernel has just past its 32-nd year birthday.[^1] In many devices including web servers, desktop computers and mobile devices, you can find Linux kernel.

Linux kernel is not easy to manage, so people create and add many components and release various distributions.

Today, we will help you to install a Linux Desktop distribution on your computer. You can choose Ubuntu, one of popular Linux distributions, or a Debian based distribution which is developed to be used for JI courses. Also you can choose other distributions.

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
3. Install git, compiles and other tools you want to use by `apt`.

---
# Well known tools you could use in Linux
- Chrome, Edge, 360 Browser ... -> Firefox
- Microsoft Office -> Libre office, WPS(not opensource)
- App store -> apt (and many UI store integrated with apt)
- Chinese Input system -> Sogou Pinyin, Rime

[^1]: https://www.phoronix.com/news/Linux-6.6-rc2-Released