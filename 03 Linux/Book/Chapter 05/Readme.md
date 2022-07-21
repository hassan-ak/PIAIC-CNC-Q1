# Chapter Five: Post-Installation Activities

## 5.1 Managing Hardware and Peripherals

### 5.1.1 CPU

- The operating system keeps programs and hardware working together smoothly
- The capabilities of Linux are affected by the limitations of your system’s hardware (for example, disk space and memory) so it is important to know more details about your computer’s hardware
- Let’s start with the central processing unit (CPU)
- The CPU performs all the computing and its speed (in MHz) signifies how fast your computer can handle transactions
- Your CPU specs will also tell you about the CPU family (most common are x86 and x86-64) and the number of “cores” that it has
- To increase performance, manufacturers add additional “cores,” or central processing units
- For example a dual-core CPU has two central processing units, quard core has 4 central processing units so it appears to the operating system as two/four CPUs
- A CPU with two cores, for example, could run two different processes at the same time.
- This speeds up your system, because your computer can do multiple things at once

| Command | Argument     | Description                                       |
| ------- | ------------ | ------------------------------------------------- |
| uname   | -a           | Print all information (machine, processer and OS) |
| lscpu   |              | Display information about the CPU architecture    |
| cat     | proc/cpuinfo | CPU detailed info                                 |

### 5.1.2 Hard Disk

- If you plan on adding a new disk in the future, learning how to partition will come in handy
- A disk partition or partition is a section of the hard drive that is separated from other segments
- Partitions enable users to divide a physical disk into logical sections, For example C Drive, D Drive etc in windows operating system
- Linux supports the following partitioning tools
  - Fdisk Tools
    - This is composed of the text-based tools:
      - fdisk
      - cfdisk
      - sfdisk
    - These tools are great for use in partitioning. However, it could be a bit overwhelming for beginners who are not yet familiar with partitioning
  - libparted Tools
    - The libparted library presents both GUI and text-based partitioning tools
    - GParted is a one of the free partition editor which can be downloaded and installed for graphically managing your disk partitions
    - The interface makes it easier to use for beginners
  - GPT fdisk Tools
    - These are tools created for GPT (Globally Unique Identifier Partition Table) disks using the fdisk tools
    - The GUID Partition Table (GPT) is a standard for the layout of partition tables of a physical computer storage device, such as a hard disk drive or solid-state drive, using globally unique identifiers (GUIDs)

| Command | Argument         | Description                                                                                             |
| ------- | ---------------- | ------------------------------------------------------------------------------------------------------- |
| df      | df               | Get a full summary of available and used disk space usage of the file system.                           |
| df      | -h               | Get a full summary of available and used disk space usage of the file system (human readable form)      |
| du      | du               | Check the information of disk usage of files and directories on a machine                               |
| du      | -h \| less       | Check the information of disk usage of files and directories on a machine (human readable page by page) |
| du      | <directory_path> | Check the information of disk usage of directories for a specific path                                  |
| du      | -s               | Check the information of disk usage of directory                                                        |

### 5.1.3 Removable Storage

- Using storage such as USB flash drives and external hard disks in Linux works similarly when using Windows or Mac OS
- Plug the device in and Linux will detect the device
- Aside from accessing the drive via the desktop GUI, you can also navigate to the /media directory and find the mounted subdirectory
- After you use the removable media, unmount the disk before removing it to avoid any disk issues
- You can generally right-click on the Device Name and click on any of the options such as Unmount, Eject Volume, or Safely Remove

### 5.1.4 USB Devices

- You can connect other devices such as I/O devices (keyboard, mouse), cameras, mobile phones, scanners and printers to your Linux computer and expect that these work in a plug-and-play manner
- For printers, you will also need to set up the printer configuration after Linux detects the device

## 5.2 Installing Additional Software

- Linux-compatible softwares come in
  - .rpm for RPM packages (Fedore, SUSE)
    - RPM Package Manager (also known simply as RPM), originally called the Red-hat Package Manager, is a program for installing, uninstalling, and managing software packages in Linux
    - The .rpm files are used primarily by distributions that derive from Redhat based distros (Fedora, CentOS, RHEL) as well as by the openSuSE distro
  - .deb for Debian packages (Debian, Ubuntu, Xandros)
    - A file with the DEB extension is a Debian Software Package file
    - The .deb files are meant for distributions of Linux that derive from Debian (Ubuntu, Linux Mint, Xandros etc.)
    - They're used mainly in Unix-based operating systems, including Ubuntu and iO
- Both of the file with either .deb and .rpm are more akin to a .zip file
- Even if the type of packages varies, both RPM and Debian packages can be installed in any type of Linux distribution
- Popularly used distributions provide a GUI for installing additional applications
- In Ubuntu you can use “Ubuntu Software” to find any app you want to install
- Ubuntu Software is similar to Play Store and App Store we have in android and iOS

### 5.2.1 Installing Applications in Ubuntu

| Command   | Argument                      | Description                                      |
| --------- | ----------------------------- | ------------------------------------------------ |
| apt-cache | search <keyword>              | Display all packages available against a keyword |
| apt-get   | update                        | Fetch updated packages from source               |
| apt-get   | upgrade                       | Install updated packages                         |
| apt-get   | install <package_name>        | Install a package                                |
| apt       | install <package_name>        | Install a package                                |
| apt       | remove <package_name>         | Remove package                                   |
| apt       | --purge remove <package_name> | Remove package along with configration files     |
| apt       | list --installed              | List all installed packages                      |

### 5.2.2 Installing Applications in Fedora

- rpm packages are used
