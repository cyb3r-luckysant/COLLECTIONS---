# Linux Commands and System Information Guide 🐧

Welcome to the comprehensive guide to essential Linux commands and system information! This document, curated by **cyb3r-luckysant**, will help you navigate through the most important Linux commands, covering everything from file management to system monitoring. 🚀

---

## Table of Contents 📑

1. [Basic File Operations 📂](#basic-file-operations)
2. [System Information 🖥️](#system-information)
3. [Package Management 📦](#package-management)
4. [Process Management ⚙️](#process-management)
5. [User and Group Management 👤](#user-and-group-management)
6. [Networking and Connectivity 🌐](#networking-and-connectivity)
7. [Searching and File Finding 🔍](#searching-and-file-finding)
8. [Disk Management 💾](#disk-management)
9. [Security and Permissions 🔒](#security-and-permissions)
10. [System Monitoring 📊](#system-monitoring)
11. [Miscellaneous Commands 🛠️](#miscellaneous-commands)

---

## 1. Basic File Operations 📂

### 1.1 Listing and Navigating

- `ls`: List files and directories in the current directory.
- `cd <directory>`: Change the current directory.
- `pwd`: Display the current working directory.

### 1.2 File Manipulation ✂️

- `touch <filename>`: Create an empty file or update the timestamp of an existing file.
- `cp <source> <destination>`: Copy files or directories.
- `mv <source> <destination>`: Move or rename files and directories.
- `rm <file>`: Delete a file.
- `rmdir <directory>`: Remove an empty directory.
- `rm -r <directory>`: Remove a directory and its contents recursively.

### 1.3 File Viewing and Editing ✍️

- `cat <file>`: Display the entire content of a file.
- `less <file>`: View file content interactively (allows scrolling).
- `head <file>`: Display the first 10 lines of a file.
- `tail <file>`: Display the last 10 lines of a file.
- `nano <file>`: Edit a file using the nano text editor (or `vi`, `vim`).

---

## 2. System Information 🖥️

### 2.1 General System Info

- `uname -a`: Display detailed system information (kernel, architecture, etc.).
- `lsb_release -a`: Show Linux distribution information.
- `hostname`: Display or set the system hostname.
- `uptime`: Show system uptime, load averages, and current time.
- `arch`: Display the machine's architecture.

### 2.2 CPU, Memory, and Disk Info

- `top`: Interactive process viewer (real-time stats for CPU, memory usage).
- `htop`: An enhanced version of `top` with better user interface (requires installation).
- `free -h`: Display free and used memory in human-readable format.
- `df -h`: Show disk space usage for mounted filesystems.
- `du -sh <directory>`: Show the total size of a directory.

---

## 3. Package Management 📦

### 3.1 Debian/Ubuntu-based Systems

- `sudo apt update`: Update the list of available packages.
- `sudo apt upgrade`: Upgrade installed packages.
- `sudo apt install <package>`: Install a package.
- `sudo apt remove <package>`: Remove a package.
- `sudo apt autoremove`: Remove unused packages.
- `sudo apt-cache search <package>`: Search for a package.

### 3.2 Red Hat/Fedora/CentOS-based Systems

- `sudo dnf update`: Update system packages.
- `sudo dnf install <package>`: Install a package.
- `sudo dnf remove <package>`: Remove a package.
- `sudo dnf search <package>`: Search for a package.

---

## 4. Process Management ⚙️

### 4.1 Viewing Processes 👀

- `ps aux`: List all running processes.
- `top`: Display real-time system resource usage and process list.
- `htop`: An enhanced process viewer with a graphical interface (requires installation).
- `pgrep <process_name>`: Search for a process by name.
- `pidof <process_name>`: Display the PID of a running process.

### 4.2 Managing Processes 🛠️

- `kill <PID>`: Terminate a process by PID.
- `killall <process_name>`: Terminate processes by name.
- `bg <job_number>`: Resume a paused job in the background.
- `fg <job_number>`: Bring a job to the foreground.
- `nice -n <priority> <command>`: Start a command with a specific priority (lower value = higher priority).
- `renice <priority> <PID>`: Change the priority of an existing process.

---

## 5. User and Group Management 👤

### 5.1 User Management

- `whoami`: Display the current logged-in username.
- `id <username>`: Display user and group ID information.
- `adduser <username>`: Create a new user.
- `usermod -aG <group> <username>`: Add a user to a group.
- `passwd <username>`: Change a user's password.
- `deluser <username>`: Delete a user account.

### 5.2 Group Management

- `groupadd <group_name>`: Create a new group.
- `groupdel <group_name>`: Delete a group.

---

## 6. Networking and Connectivity 🌐

### 6.1 Network Configuration

- `ifconfig`: Display or configure network interfaces (deprecated, use `ip`).
- `ip a`: Display all network interfaces and their IP addresses.
- `ip link set <interface> up/down`: Enable or disable a network interface.
- `hostname -I`: Display the IP address of the system.

### 6.2 Network Testing 🧪

- `ping <hostname>`: Send ICMP echo requests to test connectivity.
- `traceroute <hostname>`: Trace the route packets take to a destination (requires installation).
- `netstat -tuln`: Show active network connections and listening ports.
- `ss -tuln`: Display socket statistics (more modern than `netstat`).
- `curl <URL>`: Fetch data from a URL or test HTTP connections.

---

## 7. Searching and File Finding 🔍

### 7.1 Finding Files

- `find <path> -name <filename>`: Search for files by name.
- `locate <filename>`: Search for a file using the pre-built database.
- `updatedb`: Update the database used by `locate`.

### 7.2 Searching within Files 📄

- `grep <pattern> <file>`: Search for a pattern within a file.
- `grep -r <pattern> <directory>`: Recursively search for a pattern in a directory.
- `ag <pattern>`: Search within files (faster than `grep` with "The Silver Searcher" installed).

---

## 8. Disk Management 💾

### 8.1 Disk and Partition Information

- `lsblk`: List information about all block devices.
- `fdisk -l`: List disk partitions.
- `blkid`: Show block device attributes (like UUIDs).
- `mount <device> <mount_point>`: Mount a disk or partition.
- `umount <mount_point>`: Unmount a device or partition.

### 8.2 Disk Usage 📊

- `df -h`: Display disk space usage.
- `du -sh <directory>`: Show the total disk usage of a directory.

---

## 9. Security and Permissions 🔒

### 9.1 File Permissions

- `chmod <permissions> <file>`: Change the permissions of a file or directory.
- `chown <user>:<group> <file>`: Change the ownership of a file or directory.
- `chgrp <group> <file>`: Change the group of a file or directory.

### 9.2 User Authentication

- `sudo <command>`: Execute a command as another user (usually root).
- `sudo su`: Switch to the root user.
- `visudo`: Edit the sudoers file safely.

---

## 10. System Monitoring 📊

### 10.1 System Performance

- `top`: Display real-time system stats (CPU, memory, etc.).
- `vmstat`: Show system performance information (memory, processes, etc.).
- `sar`: Collect, report, and save system activity information.
- `iotop`: Monitor I/O usage by processes (requires installation).

### 10.2 Log Files 📜

- `journalctl`: View system logs (for `systemd` systems).
- `dmesg`: Display boot and system-related messages.

---

## 11. Miscellaneous Commands 🛠️

- `echo <text>`: Print text to the terminal.
- `history`: Show command history.
- `alias <name>='<command>'`: Create an alias for a command.
- `man <command>`: Show the manual page for a command.
- `exit`: Exit the current terminal session.

---

<br>

### 👨‍💻 Author  
Developed by **Cyb3r-LuckySant** ❤️  
