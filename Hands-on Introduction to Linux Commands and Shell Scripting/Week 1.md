## Course Introduction
- Explore all aspects of scripts
- explore bash shell scripting
- discover useful features of the bash shell
- Module 1. Introduction to Linux

Module 2. Introduction to Linux Commands

Module 3. Introduction to Shell Scripting

Module 4. Final Project and Final Exam

	Lesson 1. Practice Project

	Lesson 2. Final Project

	Lesson 3. Final Exam
 
## Introducing Linux and Unix
- os is a software that manages hardware and provides interaction between user and hardware.
- UNIX is a family of operating systems.
- LINUX is a family of Unix-like operating systems.
- 

## Linux Distributions
- distribution is a specific flavor of the Linux os also referred to as distro
- Debian distro
- Ubuntu distro
- Linux distro" -- is a version of the open-source Linux operating system that is packaged with other components, such as installation programs, management tools, and additional software such as the KVM hypervisor.
- red hat distro
- fedora
- suse
- arch linux

## Overview of Linux Architecture
- 5 layer
- UI layer - user interface
- applcication layer - system daemons, shells, users apps =, tools ---- these are softwares that allow user to perform certain task
- os -- controls the jobs and programs... 
- kernel --- performs the most vital operations.. lowest level software... acts as a bridge bw apps and computer hardware. ( key jobs - memory management, process management, managing device driver.)
- hardware -- includes CPU, ram, storage, screen, and USB devices.
- top level of the file system is the root directory. /
- key directory in Linux is /bin
- /usr
- /home
- /boot
- /media
-  A Linux system consists of five key layers.
-  The user interface is the layer that enables the user to interact with applications using control devices​.
-  Applications enable users to perform certain tasks within the system.
-  The operating system runs on top of the Linux kernel and is vital for system health and stability.
-  The kernel is the lowest-level software and enables applications to interact with your hardware.
-  Hardware includes all the physical or electronic components of your PC. And the Linux filesystem is a tree-like structure consisting of all directories and 
   files on the system.

## Linux Terminal Overview
- Linux shell is an os level application that interprets commands.
- ~ home directory   cd ~
- / root directory   cd /
- .. parent of the current directory
- current directory
- cd - to change the directory
- bin directory is inside roots which contain programs required by the system.
- pwd commands prints the present path name.
- ls - shows the list of all the content in the present working directory.
- ls /home
- root directory is denoted by  /
- ls /
https://www.coursera.org/learn/hands-on-introduction-to-linux-commands-and-shell-scripting/ungradedWidget/8IMo5/reading-browsing-directories-with-the-linux-terminal 


## Creating and Editing Text Files
- popular text editor in linux
- command line text editors and gui text editors
- gnu nano, vi, vim
- gedit - integrated file browser, syntax color coding
- emacs
- nano <filename>
- vim <filename> -- insert mode and command mode
- :sav example.txt to create a file and write the buffer to the file
- :w to write the buffer to the file without exiting
- :q to quit vim session
- :q! to quit without saving

- Use the sudo command to enable access to "super-user" system administration tools
- Use the apt system administration command to update and install two popular packages for text editing: nano and Vim
- Create and edit files using nano
- Create and edit files using Vim
- sudo apt update --  update your package list index
- sudo apt upgrade nano -- 

## Installing Software and Updates
- package and package managers
- Dev and RPM packages
- .deb for debian based
- .rpm for red hat based like fedora
- rpm to deb --- alien <package_name>.rpm
- deb to rpm --- alien -r <package_name>.deb
- apt is a linux tool to update deb based linux system
- yum is a command to update rmp based system
- sudo apt update package.name
- pip install pandas -- pip package manager to check and install
- 
