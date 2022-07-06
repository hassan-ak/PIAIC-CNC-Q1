# CNC - Yousaf - 2022/06/26

## Linux for Beginners

### Agenda

1. Getting Started
2. Understanding Linux
3. Your First Linux Experience
4. Post Installation Activities
5. Using the Linux Command Line
6. Basic Administration & Security
7. Introduction to Scripting

### Chapter 1: Getting Started

- Overview of Linux
- Differences with Other OS

#### 1.1 What is an Operating System?

- A special kind of software which is between the hardware of the PC and the programs that you want to use and work with.
- The OS is the software that brings together the a computer’s hardware and the different programs you want to install on it.

##### 1.1.1 The OS is responsible for the following tasks:

1. Detect hardware
   - An OS is responsible for validating the components of a computer during boot up and loading the corresponding drivers and modules for the hardware to properly run.
2. Manage processes
   - Similar to the way our mind works, several processes or applications are running on a computer at the same time.
   - It is the OS that is responsible for allocating CPU resources and sharing it among the processes.
   - The OS also provides the user the option to start, stop, or restart a process.
3. Manage memory
   - Each application needs a specific amount of RAM and swap memory to function.
   - The OS is responsible for assigning memory allocations and for handling memory requests.
4. Initiate user interfaces
   - An OS offers users ways to access the system either via a command line or a graphical user interface (GUI).
5. Establish file systems
   - An OS offers users ways to access the system either via a command line or a graphical user interface (GUI).
6. Manage access and user authentication
   - An OS allows for creating user accounts with different permissions for access to files and processes.
7. Provide a platform for administrative use
   - A computer’s OS provides a platform for the administrator to add users, allocate disk space, install software, and to perform activities to manage the computer.
8. Startup-services
   - The OS manages several processes running in the background known as daemon processes.

#### 1.2 What is Linux?

- Linux is Open-Source
  - Linux is continuously developed collaboratively.
  - No single company owns the development and support of Linux.
- There are more than 100 companies and over 1,000 developers who work together for every kernel release.
- Kernel
  - Linux is composed of a kernel, the core control software, plus plenty of libraries and utilities that provide different features.
- Distributions
  - Linux is available in many distributions.
  - These are called Linux flavors.
  - Distributions are groups of specific kernels and programs.
  - Arch, SUSE, Ubuntu, and Red Hat
- Linux has the largest market share when it comes to server OS
- Least popular for personal and home use

##### 1.2.1 Linux has the following additional characteristics:

1. Supports clustering
   - Multiple Linux systems can be configured to appear as one system from the outside.
   - Service can be configured among clusters and still offer a seamless experience.
2. Runs virtualization
   - Virtualization allows one computer to appear as several computers to users.
   - Linux can be configured as a virtualization host - where you can run other OS such as Windows, macOS, or other Linux systems.
   - All the virtualized systems appear as separate systems to the outside world
3. Cloud computing
   - Almost all cloud servers run on Linux.
4. Options for storage
   - Data need not always be stored in your hard disk.
   - Linux offers different local and networked storage options such as Fiber Channel and iSCSI.

#### 1.3 History of Linux

- Linus Torvalds
  - A student from Finland, he created Linux in 1991 using C and assembly language.
  - Initially, he named it Freax, a combination of the words “Free” + “Freak” + “x”
- Ari Lemmke
  - He was the FTP server administrator where Linus uploaded the files for the operating system.
  - He didn’t think Freax sounded good so he renamed the folder to Linux without telling Linus.
- GNU GPL License
  - In 1992, Linux was licensed under the GNU GPL and the first Linux distributions (also called distro) were created.
  - GPL = General Public License
- Slackware
  - The oldest existing Linux distro
- Debian
  - The largest community distribution
- Suse & Red Hat
  - Commercial distributions
- Market Share
  - Server market revenue has already passed that of UNIX.
  - Android mobile OS has gained 75% market share.
- 98.8% of the world’s fastest systems use the Linux kernel.

#### 1.4 Linux as Compared to other Operating Systems

1. Cost
   - Windows, if obtained legally, costs at least $100 and even more for the Pro and Commercial versions.
   - Linux is free of charge, even for commercial distros.
   - Companies sell services for support and documentation but not for the software.
2. Viruses
   - Linux hardly gets any viruses.
   - Since most people use Windows, attackers target windows.
   - Since its open-source, more developers are able to look for security flaws and help with fixes.
3. System Stability
   - Large scale systems can go for years without restarting the server.
   - Only time when restart is needed is kernel updates.
   - Even upgrading software only requires a service restart, not a node restart.
4. Installation
   - Basic software is provided with Linux OS installation:
     - Text Editor
     - Spreadsheet
     - Presentation Program
     - Photo Editor
     - Web Browser
     - Movie Player
     - PDF Reader
   - Drivers are pre-installed and configured with the install
5. Support
   - Large online community:
     - Get information
     - Read FAQs
     - Ask Questions
   - Unlimited number of resources to use and learn from.
   - All for free.

##### 1.4.1 Stick to yourcurrent OS if these conditions apply:

- You need to use proprietary software and cannot find an open-source equivalent
- If you are a serious gamer. Most PC games are made for Windows.
- Hardware compatibility issues - many hardware devices don’t come with Linux drivers
