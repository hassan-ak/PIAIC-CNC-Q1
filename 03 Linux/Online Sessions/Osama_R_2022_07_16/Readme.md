# CNC - Osama - 2022/07/16

## Linux for Beginners

### Chapter Four: Your First Linux Experience

#### 4.2 Getting to Know Shell

- Linux distribution uses the root username for administrator access
- The desktop that comes up is either KDE or GNOME
- The GUI for KDE or GNOME provides the best way to explore Linux through icons, windows, and pointers
- Alternate to it is Terminal / Console window
- If you notice image above in which you will find `aamir@ap-linux:~$`
- This is called shell
- The shell is where you can run executable files and shell scripts.
- The shell is also what we call the command line. Commands are written using the general syntax below: `command option1 option2 . . . optionN`
- uptime is the command that shows the duration that the computer has been up.
- uname is the command to show the operating system name.
  - s (print the operating system name),
  - r (print the operating system release),
  - v (print the operating system version) are options that you can use for the uname command
- To know about the options that you can use for a particular command, you can use the man command
- In computing, the superuser is a special user account used for system administration
- The root user can do many things an ordinary user cannot for example install new software, removing any existing application, making change in any system settings etc.
- Depending on the operating system (OS), the actual name of this account might be root, administrator, admin or supervisor
- To switch to root while in the shell, enter the command su - and then input your root password
- Changing to root password while in the shell environment will allow you to run tasks

#### 4.3 Linux Desktops

- There are two commonly used GUIs that come with Linux distributions:
  - GNOME
    - Acronym for GNU Network Object Model Environment. (Pronounced guh-nome)
    - GNOME is a Windows-like desktop system that works on UNIX and UNIX-like systems and is not dependent on any one window manager
  - KDE
    - Acronym for K Desktop Environment
    - KDE GUI is equipped with everything users typically need, including a file manager, window manager, help tool and system configuration tool
- You can have both installed in your computer and switch between the two whenever you want to
- Both GUIs also run on Unix, and while there are other GUIs that can be installed on Linux, these two remain as the most popular in use

| Criteria                                                         | GNOME                                                                                                                               | KDE                                                                                                                                                                     |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Availability                                                     | Free                                                                                                                                | Free                                                                                                                                                                    |
| Minimum System Requirements                                      | 700 MHz CPU, 768 MB RAM                                                                                                             | 1 Ghz CPU, 615 MB RAM                                                                                                                                                   |
| Development Priorities                                           | Focuses on freedom, accessibility, and developer-friendliness                                                                       | Provides an aesthetically pleasing website with great configurability                                                                                                   |
| Customization Experience                                         | The interface is simple to use and great for first-time Linux users, advanced users may find its customization settings as limiting | Allow for versatile configuration that creates great looking desktop, but the user has to learn to navigate the options. Customization makes it more resource-intensive |
| Default appearance (Note that both offers customization options) | Default setting: Toolbar at the top and a dock that pops out featuring application icons                                            | Default setting: toolbar at the bottom and a main menu.                                                                                                                 |
| Universal Search                                                 | Uses text-based search functionality                                                                                                | Uses text-based and menu-based navigation                                                                                                                               |
| Resource Usage and User Experience                               | Less resource-intensive than KDE                                                                                                    | Good for users who came from Windows OS                                                                                                                                 |

#### 4.4 Navigating the Linux Filesystem

- Linux organizes files using a hierarchical system
- Files are stored in directories and these directories can also contain other directories
- When you compare the Linux filesystem to Windows, you will find that there are no drive letters in Linux
- All files are stored in a single root directory noted as “/” regardless of where the data is physically stored (hard drive, external drive, or CR-ROM).
- To find a file in Linux, you also need the information about the directory hierarchy known as the pathname

| Sr. No. | Path        | Files Contained                                                               |
| ------- | ----------- | ----------------------------------------------------------------------------- |
| 1       | /           | Single root directory – file system base                                      |
| 2       | /bin        | Executable files such as Linux commands cat,cp,ls                             |
| 3       | /boot       | Files that the boot loaders access during start-up–including the Linux kernel |
| 4       | /dev        | Files for the different hardware/devices                                      |
| 5       | /etc.       | Initialization scripts and system config files                                |
| 6       | /home       | User directories                                                              |
| 7       | /lib        | Library files which includes driver modules                                   |
| 8       | /lost+found | For lost files                                                                |
| 9       | /media      | Mounting removal media filesystems                                            |
| 10      | /mnt        | Temporary directory for mounted filesystems                                   |
| 11      | /opt        | For storing application packages                                              |
| 12      | /proc       | Information on Linux processes                                                |
| 13      | /root       | Root user home directory                                                      |
| 14      | /sbin       | Executable files for commands used by root user                               |
| 15      | /srv        | For services hosted by the system (e.g. FTP, web)                             |
| 16      | /tmp        | Temporary directory – deleted during system reboot                            |
| 17      | /usr        | Contains subdirectories for program files                                     |
| 18      | /var        | Log files                                                                     |

- To navigate in the directories on Linux, you can either use the
  - GUI to find a certain file by going through the folders,
  - Using the universal text-based search function,
  - By using the command line.
- You can use the following useful commands in your terminal to navigate and work in the file system:

#### Commands

| Command  | Argument                                 | Description                                                                      |
| -------- | ---------------------------------------- | -------------------------------------------------------------------------------- |
| uname    |                                          | Print system information                                                         |
| uname    | -s                                       | Print the operating system name                                                  |
| uname    | -r                                       | Print the operating system release                                               |
| uname    | -v                                       | Print the operating system version                                               |
| uname    | -a                                       | Print all information (machine, processer and OS)                                |
|          | --help                                   | help regarding a command                                                         |
| info     | <command>                                | Reads documentation in the info format (online)                                  |
| hostname |                                          | Display hostname                                                                 |
| man      | <command>                                | Display the user manual of any command that we can run on the terminal (offline) |
| su       |                                          | Switch to root user in current working directory                                 |
| su       | root                                     | Switch to root user in current working directory                                 |
| exit     |                                          | Exit root user                                                                   |
| pwd      |                                          | display the directory where you are currently in.                                |
| ls       | -a                                       | List down all the contents of a directory along with hiden files                 |
| ls       | <string>\*;                              | List down all the contents of a directory starting with string                   |
| ls       | \*<string>                               | List down all the contents of a directory ending with string                     |
| which    | <command>                                | Locate a command                                                                 |
| cp       | <file_name> <directory_path>             | Copy file to path                                                                |
| cp       | <directory_path_1> <directory_path_2> -r | Copy one directory to other                                                      |
| mv       | <file_name> <directory_path>             | Move file to path                                                                |
| mv       | <directory_path_1> <directory_path_2> -r | Move one directory to other                                                      |
| rm       | <file_name>                              | Delete a file                                                                    |
| rm       | <directory_name> -rf                     | Delete a folder with mulitple file sin it                                        |
| rm       | /                                        | Delete ubuntu                                                                    |
| find     | <directory_path> -name <file_name>       | Search a file in a directory                                                     |
| find     | <string>\*                               | Search all the files starting with string                                        |
| find     | \*<string>                               | Search all the files ending with string                                          |

#### Command Line Shortcuts

| Sr. No. | Shotcut  | Description                 |
| ------- | -------- | --------------------------- |
| 15      | ctrl + c | End running command         |
| 16      | q        | Exit from a running command |

#### Vim editor commands and shortcuts

| Command | Description    |
| ------- | -------------- |
| nyy     | copy n lines   |
| p       | paste          |
| dd      | delete         |
| u       | undo changes   |
| :x      | write and quit |

### 5.1 Managing Hardware and Peripherals

#### 5.1.1 CPU

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

##### 5.1.1 Hard Disk

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

##### 5.1.2 Removable Storage

- Using storage such as USB flash drives and external hard disks in Linux works similarly when using Windows or Mac OS
- Plug the device in and Linux will detect the device
- Aside from accessing the drive via the desktop GUI, you can also navigate to the /media directory and find the mounted subdirectory
- After you use the removable media, unmount the disk before removing it to avoid any disk issues
- You can generally right-click on the Device Name and click on any of the options such as Unmount, Eject Volume, or Safely Remove

##### 5.1.3 USB Devices

- You can connect other devices such as I/O devices (keyboard, mouse), cameras, mobile phones, scanners and printers to your Linux computer and expect that these work in a plug-and-play manner
- For printers, you will also need to set up the printer configuration after Linux detects the device

#### 5.2 Installing Additional Software

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

##### 5.2.1 Installing Applications in Ubuntu

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

##### 5.2.2 Installing Applications in Fedora

- rpm packages are used

### Chapter Seven: Using the Linux Command Line

#### 7.1 Using the Shell Features

Previously we’ve been learned few command that we also tried on Shell / Command line
We will further learn different commands that you can use in Linux, and also study the different shell features
You have now seen the capabilities of using the Bash shell
Performing tasks on the command line take less time than doing it in the GUI
To further enjoy the convenience of using the CLI (command line interface), here are some shell features that you should use:
Command Completion: You can use TAB key to complete any unfinished command
apt-ca TAB - It will automatically make it apt-cache
DOUBLE-TAB will list all the available options on the screen
Command History: Linux remembers commands you have recently typed in so you no longer need to retype

| Command          | Description                                                                    |
| ---------------- | ------------------------------------------------------------------------------ |
| Arrow Up/Down    | Display the previous commands from the more recent going to the oldest entered |
| Arrow Right/Left | Moves the cursor one character to the right/left                               |
| CTRL key + A     | Transfers cursor to the beginning of the line                                  |
| CTRL key + E     | Transfers cursor to the end of the line                                        |
| Delete key       | The character under the cursor is deleted                                      |
| Backspace        | The character to the left of the cursor is removed                             |
| CTRL key + R     | Search for a particular command from the command history.                      |

#### 7.2 Essential Linux Commands

##### 7.2.1 Help Commands

| Command | Description                                                  |
| ------- | ------------------------------------------------------------ |
| Info    | Shows online information about a command                     |
| Man     | Shows details of a command                                   |
| whatis  | Shows a short description of a specific keyword              |
| Type    | Shows the location of a command file                         |
| Alias   | Assign a command alias – especially useful for long commands |
| unalias | Remove command alias                                         |

##### 7.2.2 Managing Files and Directories

| Command | Description                               |
| ------- | ----------------------------------------- |
| Cd      | Change directory                          |
| Pwd     | Displays the current directory            |
| Ln      | Create links to files and directories     |
| touch   | To trigger a file stamp update for a file |

##### 7.2.3 Finding Files

| Command | Description                                                   |
| ------- | ------------------------------------------------------------- |
| Find    | Search for a file based on the name                           |
| whereis | Search for executable files                                   |
| which   | Search for files in the directories part of the PATH variable |

##### 7.2.3 Processing Files

| Command | Description                                                                     |
| ------- | ------------------------------------------------------------------------------- |
| Dd      | Copy lines of data                                                              |
| Diff    | Display the results of comparing two files                                      |
| More    | Show a text file one page at a time – display can only go forward               |
| Less    | Show a text file one page at a time – display can only go forward and backwards |
| Wc      | Display the count of the number of characters, words, and lines in a file       |
