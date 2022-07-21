# Chapter Seven: Using the Linux Command Line

## 7.1 Using the Shell Features

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

## 7.2 Essential Linux Commands

### 7.2.1 Help Commands

| Command | Description                                                  |
| ------- | ------------------------------------------------------------ |
| Info    | Shows online information about a command                     |
| Man     | Shows details of a command                                   |
| whatis  | Shows a short description of a specific keyword              |
| Type    | Shows the location of a command file                         |
| Alias   | Assign a command alias – especially useful for long commands |
| unalias | Remove command alias                                         |

### 7.2.2 Managing Files and Directories

| Command | Description                               |
| ------- | ----------------------------------------- |
| Cd      | Change directory                          |
| Pwd     | Displays the current directory            |
| Ln      | Create links to files and directories     |
| touch   | To trigger a file stamp update for a file |

### 7.2.3 Finding Files

| Command | Description                                                   |
| ------- | ------------------------------------------------------------- |
| Find    | Search for a file based on the name                           |
| whereis | Search for executable files                                   |
| which   | Search for files in the directories part of the PATH variable |

### 7.2.3 Processing Files

| Command | Description                                                                     |
| ------- | ------------------------------------------------------------------------------- |
| Dd      | Copy lines of data                                                              |
| Diff    | Display the results of comparing two files                                      |
| More    | Show a text file one page at a time – display can only go forward               |
| Less    | Show a text file one page at a time – display can only go forward and backwards |
| Wc      | Display the count of the number of characters, words, and lines in a file       |
| Cat     | Show a text file in one output                                                  |
| Cut     | Get sections of text in a file                                                  |
| Grep    | Display results of finding expressions in a file                                |
| Sed     | Perform editing commands, then copy to a standard output                        |
| Split   | Specify a size to break a file into                                             |
| Sort    | Arrange the lines in a file                                                     |
| Uniq    | Keep unique lines in a file and delete duplicates                               |

### 7.2.4 Compressing a File

| Command    | Description                                                              |
| ---------- | ------------------------------------------------------------------------ |
| Compress   | Use to compress a file                                                   |
| Uncompress | If a file was compressed with a compress command, use this to decompress |
| Gunzip     | Use GNU Zip to decompress files                                          |
| Gzip       | Compress files with GNU Zip                                              |
| Tar        | Archive files with one or more directories                               |

### 7.2.5 Date and Time

| Command | Description                                       |
| ------- | ------------------------------------------------- |
| Cal     | Show the calendar for the specified month or year |
| Date    | Show/Set the current date and time                |

### 7.2.6 Managing Processes

| Command  | Description                                          |
| -------- | ---------------------------------------------------- |
| Bg       | Run a program or a process in the background         |
| Free     | Check for the free memory                            |
| Kill     | Stop a process                                       |
| Nice     | Run a program with a low priority                    |
| Ps       | Show current running processes                       |
| Top      | Show list of CPU and memory utilization of processes |
| Reboot   | Restart the computer                                 |
| Shutdown | Turn off computer                                    |
