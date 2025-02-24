# Ubuntu Cheat Sheets:
| Title    | Remark  |
| -------------| -----|
| [Installation](https://github.com/potatoscript/ubuntu/wiki/Installation) | Step-by-step guide on installing Ubuntu on WSL2, Virtual Machines, or bare-metal hardware.  |
| [Basic Command](https://github.com/potatoscript/ubuntu/wiki/Basic-Command) | Fundamental Linux commands for navigating the filesystem, managing directories, and executing essential tasks.  |
| [File Management](https://github.com/potatoscript/ubuntu/wiki/File-Management) | Instructions on creating, copying, moving, deleting, and viewing files and directories using command-line utilities.  |
| [User Management](https://github.com/potatoscript/ubuntu/wiki/User-Management) | Managing user accounts, groups, permissions, and authentication settings within Ubuntu.  |
| [Permissions](https://github.com/potatoscript/ubuntu/wiki/Permissions) | Explanation of file and directory permissions, ownership, and access control mechanisms.  |
| [Process Management](https://github.com/potatoscript/ubuntu/wiki/Process-Management) | Monitoring and controlling system processes, jobs, and background tasks using command-line tools.  |
| [Networking](https://github.com/potatoscript/ubuntu/wiki/Networking) | Configuring and troubleshooting network interfaces, checking connectivity, and managing network services.  |
| [Package Management](https://github.com/potatoscript/ubuntu/wiki/Package-Management) | Installing, updating, removing, and managing software packages using APT, Snap, and Flatpak.  |
| [System Monitoring](https://github.com/potatoscript/ubuntu/wiki/System-Monitoring) | Tools for tracking CPU, memory, disk usage, and overall system performance in real-time.  |
| [Disk Management](https://github.com/potatoscript/ubuntu/wiki/Disk-Management) | Partitioning, formatting, mounting, and monitoring storage devices and disk space.  |
| [Services & Daemons](https://github.com/potatoscript/ubuntu/wiki/Services-and-Daemons) | Managing system services, background processes, and startup programs using systemd.  |
| [Firewall & Security](https://github.com/potatoscript/ubuntu/wiki/Firewall-Security) | Configuring Ubuntu’s firewall, securing SSH access, and implementing best security practices.  |
| [Environment Variables](https://github.com/potatoscript/ubuntu/wiki/Environment-Variables) | Setting, modifying, and managing environment variables for system and user sessions.  |
| [Shell Scripting](https://github.com/potatoscript/ubuntu/wiki/Shell-Scripting) | Writing and executing Bash scripts to automate repetitive tasks and streamline system operations.  |
| [Cron Jobs & Automation](https://github.com/potatoscript/ubuntu/wiki/Cron-Jobs-Automation) | Scheduling and automating tasks using cron jobs, systemd timers, and task automation tools.  |
| [Docker & Containers](https://github.com/potatoscript/ubuntu/wiki/Docker-Containers) | Deploying and managing containerized applications using Docker, Podman, and Kubernetes.  |
| [Virtualization](https://github.com/potatoscript/ubuntu/wiki/Virtualization) | Running virtual machines on Ubuntu using KVM, QEMU, VirtualBox, and Vagrant.  |
| [Git & Version Control](https://github.com/potatoscript/ubuntu/wiki/Git-Version-Control) | Managing code repositories, version control workflows, and collaboration using Git.  |
| [Python & Development](https://github.com/potatoscript/ubuntu/wiki/Python-Development) | Setting up Python, virtual environments, package management, and development tools.  |
| [Node.js & JavaScript](https://github.com/potatoscript/ubuntu/wiki/NodeJS-JavaScript) | Installing Node.js, managing dependencies with npm/yarn, and running JavaScript applications.  |
| [Database Management](https://github.com/potatoscript/ubuntu/wiki/Database-Management) | Installing and managing databases such as MySQL, PostgreSQL, SQLite, and MongoDB.  |
| [System Backup & Recovery](https://github.com/potatoscript/ubuntu/wiki/System-Backup-Recovery) | Strategies for backing up, restoring, and recovering system data and configurations.  |
| [Remote Access & SSH](https://github.com/potatoscript/ubuntu/wiki/Remote-Access-SSH) | Securely connecting to remote machines using SSH, SCP, Rsync, and session management tools.  |
| [Logging & Debugging](https://github.com/potatoscript/ubuntu/wiki/Logging-Debugging) | Monitoring system logs, troubleshooting errors, and debugging applications effectively.  |
| [Performance Tuning](https://github.com/potatoscript/ubuntu/wiki/Performance-Tuning) | Optimizing system performance, tuning kernel parameters, and managing resource allocation.  |
| [Compiling Software](https://github.com/potatoscript/ubuntu/wiki/Compiling-Software) | Building software from source using compilers like GCC, Clang, Make, and CMake.  |
| [Linux Kernel Management](https://github.com/potatoscript/ubuntu/wiki/Linux-Kernel-Management) | Understanding and managing the Linux kernel, including updates, modules, and custom builds.  |


---

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Basic Commands](#basic-commands)
- [File Management](#file-management)
- [User and Group Management](#user-and-group-management)
- [Permissions and Ownership](#permissions-and-ownership)
- [Networking](#networking)
- [Package Management](#package-management)
- [Process Management](#process-management)
- [Disk Management](#disk-management)
- [System Services](#system-services)
- [SSH and Remote Access](#ssh-and-remote-access)
- [Firewall and Security](#firewall-and-security)
- [Automating Tasks](#automating-tasks)
- [Advanced Topics](#advanced-topics)

---

## Introduction
Ubuntu is a popular Linux distribution based on Debian. It is widely used for development, servers, and desktop computing. This tutorial provides a comprehensive guide to Ubuntu, from installation to advanced usage.

## Installation
1. Download the latest Ubuntu ISO from [ubuntu.com](https://ubuntu.com/).
2. Create a bootable USB using tools like Rufus or Balena Etcher.
3. Boot from the USB and follow the installation steps.
4. Choose installation type (Normal, Minimal, or Custom).
5. Set up user credentials and wait for the installation to complete.
6. Restart and remove the USB drive.

## Basic Commands
```bash
uname -a      # Show system information
lsb_release -a # Show Ubuntu version
hostnamectl    # Display hostname and system info
whoami         # Show current user
pwd            # Print working directory
``` 

## File Management
```bash
ls -l          # List files with details
cd /path       # Change directory
mkdir newdir   # Create a new directory
rm file        # Remove a file
cp source dest # Copy files
mv old new     # Move or rename files
find / -name filename # Search for files
``` 

## User and Group Management
```bash
who             # Show logged-in users
useradd -m user # Create a new user
passwd user     # Change user password
usermod -aG group user # Add user to a group
deluser user    # Delete a user
``` 

## Permissions and Ownership
```bash
ls -l file      # Show file permissions
chmod 755 file  # Change file permissions
chown user file # Change file ownership
chgrp group file # Change group ownership
``` 

## Networking
```bash
ip a              # Show IP addresses
ping google.com   # Test connectivity
netstat -tulnp    # Show open ports
ss -tulnp         # Show network connections
curl -I http://example.com # Fetch headers
``` 

## Package Management
```bash
sudo apt update        # Refresh package list
sudo apt upgrade       # Upgrade all packages
sudo apt install pkg   # Install a package
sudo apt remove pkg    # Remove a package
sudo apt autoremove    # Remove unused dependencies
``` 

## Process Management
```bash
ps aux            # Show running processes
top               # Display real-time process info
kill PID          # Terminate a process
killall name      # Kill a process by name
``` 

## Disk Management
```bash
df -h             # Show disk usage
lsblk             # List block devices
fdisk -l          # Show disk partitions
mount /dev/sdX /mnt # Mount a disk
umount /dev/sdX   # Unmount a disk
``` 

## System Services
```bash
systemctl list-units --type=service  # List running services
sudo systemctl start service         # Start a service
sudo systemctl stop service          # Stop a service
sudo systemctl restart service       # Restart a service
``` 

## SSH and Remote Access
```bash
ssh user@host     # Connect to a remote machine via SSH
scp file user@host:/path  # Copy file via SSH
rsync -av file user@host:/path  # Sync files via SSH
``` 

## Firewall and Security
```bash
sudo ufw status    # Check firewall status
sudo ufw enable    # Enable the firewall
sudo ufw disable   # Disable the firewall
sudo ufw allow 22  # Allow SSH
sudo ufw deny 80   # Block HTTP
``` 

## Automating Tasks
```bash
crontab -e       # Edit cron jobs
crontab -l       # List scheduled tasks
``` 

## Advanced Topics
- **Docker & Containers**
- **Virtualization with KVM/QEMU**
- **Automated Deployment with Ansible**
- **Kernel Compilation & Customization**
- **Performance Tuning & Monitoring**

---
