# ⚡ Windows Command & Tips Cheat Sheet

A curated collection of **useful Windows commands, shortcuts, and tools**.  
Perfect for admins, power-users, or anyone who wants to feel like a wizard in `cmd` or PowerShell. 🧙‍♂️

---

## 📑 Table of Contents
1. [Basic System Info](#-basic-system-info)
2. [File System & Navigation](#-file-system--navigation)
3. [Disk & File Check](#-disk--file-check)
4. [Networking](#-networking)
5. [Process & Task Management](#-process--task-management)
6. [User & Access](#-user--access)
7. [System Maintenance](#-system-maintenance)
8. [PowerShell Goodies](#-powershell-goodies)
9. [System Control & Shortcuts](#-system-control--shortcuts)
10. [Security & Monitoring](#-security--monitoring)
11. [Disk & Storage Management](#-disk--storage-management)
12. [Advanced Diagnostics](#-advanced-diagnostics)
13. [Scripting & Automation](#-scripting--automation)
14. [Keyboard Shortcuts](#-keyboard-shortcuts)
15. [Quick Fix Checklist](#-quick-fix-checklist)

---

## 🔹 Basic System Info
```bash
winver                 # Show Windows version
systeminfo             # Detailed system info (OS, uptime, RAM, etc.)
hostname               # Display computer name
driverquery            # List installed drivers
```

## 🔹 File System & Navigation
```bash
dir                    # List files in current directory
cd <path>              # Change directory
tree                   # Show folder structure
copy file1 file2       # Copy file
xcopy source dest /E/H # Copy directories (with subfolders, hidden files)
robocopy src dest /MIR # Mirror entire folders (robust copy)
```
## 🔹 Disk & File Check
```bash
chkdsk C: /f /r                      # Check and repair disk
sfc /scannow                         # Repair system files
DISM /Online /Cleanup-Image /RestoreHealth
```

## 🔹 Networking
```bash
ipconfig /all            # Detailed network info
ping example.com         # Test connectivity
tracert example.com      # Trace route to destination
netstat -ano             # Show active connections + process IDs
netstat -b               # Show which apps use these connections
```

## 🔹 Process & Task Management
```bash
tasklist                 # Show running processes
taskkill /PID <pid> /F   # Kill process by PID
taskkill /IM app.exe /F  # Kill process by name
```

## 🔹 User & Access
```bash
whoami                                   # Show current user
net user                                 # List users
net user <username> <password> /add      # Create new user
net localgroup administrators <user> /add
```

## 🔹 System Maintenance
```bash
cleanmgr              # Disk Cleanup
msconfig              # System Configuration
eventvwr              # Event Viewer
services.msc          # Manage services
```
[Others](https://github.com/yonics12/friendly-couscous/blob/main/useful-win.md)
