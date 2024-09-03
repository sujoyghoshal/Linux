# Linux Command Repository & OS Work

![Linux Logo](./linux2.png)

This repository contains a collection of essential Linux commands and scripts designed to facilitate efficient command-line usage. It also includes various projects and exercises related to introductory operating system concepts. The content is ideal for students, developers, and professionals looking to enhance their Linux skills and understanding of OS fundamentals.

---

## 1. Linux File Structure and Basic Commands

### Linux File System Structure
Linux uses a tree-like hierarchical file system structure, starting from the root directory "/". All files and directories are organized under this root directory.

### Basic Commands
- `cd /`  
  Changes the current directory to the root ("/") directory.

- `ls`  
  Lists the contents of the current directory.

- `dir`  
  Another command to list directory contents (similar to "ls").

- `mkdir <directory-name>`  
  Creates a new directory.

- `pwd`  
  Prints the current working directory path.

- `cd <directory-name>`  
  Changes the current directory to the specified directory.

- `cd ..`  
  Moves up one directory level (to the parent directory).

- `touch 1.txt`  
  Creates an empty file named "1.txt".

- `mv 1.txt <directory-name>`  
  Moves the file "1.txt" to the specified directory.

- `cp 1.txt <directory-name>`  
  Copies the file "1.txt" to the specified directory.

### GUI (Graphical User Interface)
A visual interface to interact with the system (e.g., Gnome, KDE).

### CLI (Command Line Interface)
A text-based interface to interact with the system (e.g., Bash shell).

---

## 2. Users in Linux

### Regular User
- Typically has a home directory (e.g., `/home/username`).
- Limited permissions, mainly for personal use and files.

### Root User
- The superuser with full access to the entire system.
- Can perform administrative tasks.
- Example:  
  `sudo mkdir <directory-name>`  
  Creates a directory with elevated (superuser) permissions.

### Service User
- Used for running specific services or daemons.
- Example:  
  `apache2` (web server service user).


---

## 3. Absolute Path vs. Relative Path

### Absolute Path
- Specifies the complete path from the root directory.
- Example: `/home/user/documents/file.txt`

### Relative Path
- Specifies the path relative to the current directory.
- Example: `../documents/file.txt`

---

## 4. Package Management

### Update the Package List
- `sudo apt-get update`  
  Updates the list of available packages and their versions.

### Upgrade Packages
- `sudo apt-get upgrade`  
  Installs the latest versions of all packages currently installed.

---

## 5. Listing Files and Directories

### Recursive Directory Listing
- `ls -R`  
  Lists the contents of the directory and all subdirectories.

### Hidden Files
- `touch .sujoy`  
  Creates a hidden file named ".sujoy". Hidden files in Linux start with a dot (.).
- `ls -a`  
  Lists all files, including hidden files.

### Detailed Listing with Time and Reverse Order
- `ls -lart`  
  Lists files in long format, sorted by time, and in reverse order.

![Linux File Listing](path/to/linux-file-listing-image.png)

---

## 6. Output Text to the Command Line

### Echo Command
- `echo sujoy`  
  Prints "sujoy" to the command line.

### Printf Command
- `printf "sujoy is a good boy"`  
  Prints "sujoy is a good boy" to the command line.

---

## 7. Installing Software

### Install Apache2
- `sudo apt install apache2`  
  Installs the Apache2 web server.

---

## 8. File Permissions

### Understanding Permissions
- `ls -l`  
  Displays file permissions in the format user-group-other.

### Change File Permissions
- `chmod <permissions> <file-name>`  
  Changes the file permissions using the permission number.
- Example:  
  `chmod 734 2.txt`  
  Changes the permissions of "2.txt" to "734", where:
  - 7 = Read, write, and execute for the user.
  - 3 = Write and execute for the group.
  - 4 = Read-only for others.

- Permission Numbers:  
  Use a [chmod calculator](https://chmod-calculator.com/) to determine the permission numbers.


---

## 9. System Resource and Process Management

### Top Command
- `top`  
  Displays a real-time view of system resource usage.

### Process Status
- `ps`  
  Lists currently running processes.

### All Background Processes
- `ps -a`  
  Displays all background processes.

### Kill a Process
- `kill <process-id>`  
  Terminates the specified process.

---

## 10. Switching to Superuser

### Regular User to Superuser
- `sudo su`  
  Switches from a regular user to the superuser.
- Notice the command prompt changes from "$" to "#", indicating superuser mode.
