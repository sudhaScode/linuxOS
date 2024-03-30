Open Souurce Operating System - Unix

# Unix based operating systems - top of Linux family
- macOS
- Android
- iOS
- kali linux
- ubuntu
- debian
- centos

# Components of Operating System
  - *Target Hardware* - embedded systems
  - *Kernel Development* - The kernel is the core of an OS, managing hardware interaction, memory allocation, and process scheduling. 
  - *Device Drivers* - OS needs device drivers to communicate with hardware components like disks, network cards, and displays. 
  - *User Interface(UI)* - text-based command line or a graphical user interface (GUI).  Developing a user interface involves knowledge of graphical programming frameworks and user interaction design principles.
  - *System Utilities* - file management, text editing, and process management are essential for any OS
  - *Security* -  robust memory management, secure boot processes, and user access controls to protect against vulnerabilities.

# Road map to Develop an OS
- **Planning and Design:**
    - Define the core functionalities and target user base for your OS.
    - Research existing OS architectures and open-source projects for inspiration.
    - Design the overall system architecture and component interactions.

- **Kernel Development:**
   - Start with a simple kernel or leverage an existing open-source kernel as a base.
   - Implement basic functionalities like memory management, process scheduling, and interrupt handling.
   - Ensure compatibility with your chosen hardware platform.
- **Device Driver Development:**
   -  Develop or integrate device drivers for essential hardware components.
   - Start with basic drivers for core functionalities like keyboard, display, and storage.
   - Gradually expand to support more complex hardware components.

- **User Interface Development:**
   - Choose a UI approach - text-based console or a graphical interface.
   - Develop core UI elements like menus, windows, and input handling mechanisms.
   - Consider existing UI libraries or frameworks for efficiency.

- **System Utility Development:**
  - Develop or integrate basic system utilities for file management, text editing, and process management.
  - Focus on providing essential functionalities for users to interact with the system.

- **Security Considerations:**

    - Implement security measures throughout the development process.
    - Focus on secure boot, memory management, and user access controls.
    - Continuously test and patch your OS for vulnerabilities.

- **Testing and Deployment:**

   -  Thoroughly test your OS on real hardware or emulators.
   -  Fix bugs and improve performance based on testing results.
   -  Consider a phased deployment strategy for initial user testing and feedback.



## GUI vs CLI
GUI (Graphical User Interface) and CLI (Command Line Interface) are two fundamental ways to interact with a computer system. Here's a breakdown of their key differences with examples for better understanding:
**GUI (Graphical User Interface):**
- *Visual Representation:* GUIs rely on graphical elements like windows, icons, menus, and buttons to represent information and actions. This makes them user-friendly and intuitive, especially for beginners.
- *Mouse and Keyboard Input:* GUIs primarily use a mouse to point and click on elements, although keyboard shortcuts can also be used for faster navigation.
<br> *Example:*  Most modern operating systems like Windows, macOS, and Chrome OS utilize a GUI. When you open a folder to view files, use a web browser, or interact with applications, you're using a GUI.
**CLI (Command Line Interface):**
- *Text-based Interface:* CLIs use text commands to interact with the system. Users type specific commands to perform actions, view information, or launch programs.
- *Keyboard Input:* CLIs rely solely on the keyboard for input, requiring users to type commands and arguments.
<br> *Example:* When you open a terminal window or command prompt on your computer and type commands like "ls" to list files or "cd" to change directories, you're using a CLI.

| Feature |	GUI	| CLI |
| -------: |	:-------: | :------- |		
|Interface	|Graphical |Text-based |		
|Input|	Mouse and keyboard (primary focus on mouse)|	Keyboard |		
|Learning Curve	|Easier for beginners|	Steeper learning curve for basic commands	|	
Efficiency	|Can be slower for repetitive tasks	Can be faster for experienced users	|	
Automation	|Limited	| Highly scriptable for automation		|
Error Correction| Easier to correct typos with visual cues|	Requires more precise command syntax	|


## Esential Linux Commands
### **File Manipulation and Navigation:**

- *grep:* Search for patterns within text files. Powerful for finding specific lines or content.
- *find:* Locate files based on various criteria like name, modification time, or permissions.
- *sort:* Sort files based on different criteria (lexicographically, numerically, etc.).
- *diff:* Compare the differences between two files. Essential for code version control.
- *tar:* Archive and compress files or directories into various formats (tar.gz, zip, etc.). Useful for packaging and distribution.
- *scp:* Securely copy files between remote servers using SSH. Ideal for transferring code or data across machines.
- *rsync:* Efficiently synchronize files and directories between locations, handling updates and deletions effectively.
### **System Administration and Monitoring:**

- *top:* View real-time process information, including CPU usage, memory consumption, and thread details. Helps identify resource bottlenecks and monitor system performance.
- *ps:* List running processes with detailed information like process ID (PID), username, and command arguments. Useful for troubleshooting and managing processes.
- *free:* Display information about available and used memory (RAM) on the system. Helps track memory usage and identify potential issues.
- *df:* Get information about disk usage on mounted file systems. Useful for monitoring disk space and capacity planning.
- *journalctl:* View and manage system logs. Helps diagnose system issues and track system events.
- *netstat:* Display information about network connections, including ports, protocols, and IP addresses. Useful for troubleshooting network connectivity and monitoring network activity.
### **Package Management:**

- *apt-get* (Debian/Ubuntu) or yum (Red Hat/CentOS): Search for, install, update, and remove software packages using the distribution's package manager.
- *dpkg:* Directly manage Debian packages (useful for advanced package management tasks).
- *rpm:* Directly manage RPM packages (Red Hat-based distributions).
### **Development Tools:**

- *git:* The most popular version control system for managing code changes, collaboration, and tracking project history.
- *make:* Automate build processes for software projects based on makefiles (scripts defining dependencies and build steps).
- *gcc:* GNU C Compiler. Compile C source code into executable programs.
- *gdb:* GNU Debugger. Powerful tool for debugging programs and identifying software errors.
- *python:* Execute Python scripts directly from the command line (assuming Python is installed and configured in your path).
### **Bonus Commands:**

- *man:* Access the system's manual pages for detailed information on commands, functions, and system calls. Invaluable for learning more about specific commands and their options.
- *alias:* Create custom aliases for frequently used commands to save time and improve efficiency.
- *history:* View your command history to recall previously executed commands.



## Arguments and options ## Linux Commands

*ls -a* -> to list all and hidden files inside folder
*ls -lh* - to list all contents with their size and permissions
*ls-lt* - sort the contents in the direcory in time order
*ls-ltr* - sort the contents in the direcory in time order and reverse order - odlder modified files first
- - The -a, -h, -l, -r, -t are all options supported by the ls command. They modify the output returned by ls command.
*cd* - to change directory
*pwd* - to print current working directory


*rmdir* - to delete a folder
*tree* - to print tree structure of a directory

*history* - to view command history - run the commands with their number !555 - it runs the 555th command in your history
**Commands to modify files**
**CRUD Operations** - Create, Read, Update, Delete**
- *mkdir* - to create a folder
- *touch* - to create 
- *cat* - to read a file (!wq to save and quit)
- *head* - to print head line of a file
- *tail* - to print 10 lines from head
- *more* - to print large file page by page 
- - “space” key - Go to next page
- - “b” key - Go back one page
- - “Enter” key - Show next line of content
- *echo* - to write to a file
- *rm -rf* - to delete a file
- *cp*-  to copy a file
- *mv* - to move a file
- *find* - to find a file
- *vi* - to create and 
- *vim* - to edit a file
- *nano* - to edit a file -  save a file press ctrl + o, exit the editor use ctrl +x
- *chmod* - to change file permissions

- -  Commands are used to perform different operations on a terminal (non UI)
- - Commands used while navigating file system - pwd, cd, ls
- - Relative paths can be used to easily navigate between directories
- - ~ refers to the home directory
- - . refers to the current working directory
- - .. refers to the parent working directory
- - Commands for CRUD on files and directories - mkdir, touch, cp, mv, rmdir, rm, nano
- - Commands for printing file content - cat, head, tail, more, less
# System Design
HLD and LLD

## What are Linux operating systems?
An operating system is a set of tools which makes our life easier to interact with computers eg: Go through files and folders, configure settings, connect to network etc. Windows is a commonly operating system.

Linux is a kernel (i.e, a template) based on which operating systems can be created. The linux kernel takes care of important operations like processing files, taking care of memory, cpu etc.

Here are a few Linux based operating systems (also called Linux Distributions)

1. Ubuntu
2. Debian
3. Fedora


## Linux in Real World
You are using linux servers on a daily basis, whether you realize it or not

- **Cloud applications** - Dropbox/Google drive, Other SaaS, Online streaming/gaming services
- **Mobiles, TVs, Cars, Smartwatches, Routers, Supercomputers**
- Almost all Enterprise machines

## What is command line/terminal?
- A Command Line Interface (CLI) or Terminal is a Text-based user interface (i.e, no GUI)
- Used to run programs and interact with the computer
- All GUI (Graphical User Interface) based actions eventually translate to a command in the terminal which gets executed
- The Terminal gives a direct way to run these commands
- Popular CLIs (Command Line Interface):
- - Powershell: Windows
- - Bash: Linux & MacOS

## Why you need Terminal?
  - A emulator
  -  A tool

### Absolute vs Relative paths
- Relative paths - sees forward from current directory -can be relative to home directory too. starts from /
 ![Relative path](./resources/relativepath.png)
- Absolute paths - starts from root directory



##FOSSASIA

Windows is a closed source operating system developed by Microsoft. to leavarage benifits the linux commands windows offers `WSL`. Windows Subsystem for Linux (WSL) is a feature of Windows that allows you to run a Linux environment on your Windows machine, without the need for a separate virtual machine or dual booting VM.

inatall the linux systems to windows, list all supported linux versions,
- wsl -l
After install switch to othe command line
- wsl -d Ubuntu
