# [Ubuntu Cheat Sheets](https://github.com/potatoscript/ubuntu/wiki)

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
