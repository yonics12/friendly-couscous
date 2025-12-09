# Useful Windows Command Prompt Commands

This repository contains a quick reference for useful Windows Command Prompt (`cmd.exe`) commands.  
You can use this as a cheat sheet or starting point for your own notes.

---

## 1. System & Network Information

```bat
:: Basic system info
systeminfo

:: Computer name
hostname

:: Network configuration
ipconfig
ipconfig /all

:: Release and renew IP address
ipconfig /release
ipconfig /renew

:: Clear DNS cache
ipconfig /flushdns

:: Test connectivity
ping google.com
ping 8.8.8.8

:: Trace route to a host
tracert google.com

:: Active connections and ports (with PID)
netstat -ano

:: List running processes
tasklist

:: Kill a process by PID
taskkill /PID 1234 /F
```

## 2. System & Network Information

```bat
:: Show current directory
cd

:: Change directory
cd C:\Windows
cd ..

:: Go to drive root
cd \

:: List files and folders
dir
dir /w       :: wide listing
dir /s       :: include subdirectories

```

## 3. File & Folder Management
```bat

:: Create a new directory
mkdir MyFolder

:: Remove an empty directory
rmdir MyFolder

:: Remove directory and its contents (quiet)
rmdir /S /Q MyFolder

:: Copy files
copy file.txt D:\Backup\
copy "C:\Path With Spaces\file.txt" "D:\Backup\"

:: Advanced copy (including subdirectories)
xcopy C:\Source D:\Destination /E /I

:: Robust copy (recommended for many files)
robocopy C:\Source D:\Destination /E

:: Move files or folders
move C:\file.txt D:\NewFolder\
move C:\OldFolder D:\NewFolder\

:: Delete file
del file.txt

:: Force delete, no confirmation
del /F /Q file.txt

:: Delete all .tmp files in current and subfolders
del /S /Q *.tmp

:: Rename file or folder
rename oldname.txt newname.txt
rename OldFolder NewFolder
```

## 4. Disk & System Utilities

Warning! these running with administrator

```bat
:: Check disk and fix errors (may require reboot)
chkdsk C: /F

:: System File Checker (repair system files)
sfc /scannow

:: Repair Windows image (helpful for update/system issues)
DISM /Online /Cleanup-Image /RestoreHealth

:: Disk management (use with caution)
diskpart
```

## 5. Services, Startup & Power
```bat
:: Open Services manager GUI
services.msc

:: System configuration (startup, boot options)
msconfig

:: Shut down immediately
shutdown /s /t 0

:: Restart immediately
shutdown /r /t 0

:: Log off current user
shutdown /l
```


/// end ///
