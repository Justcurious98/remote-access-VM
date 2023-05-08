# remote-access-VM
Established a Linux virtual machine, installed Open Source Initiative-approved Ubuntu images, and remotely accessed the virtual machine from a separate computer.

## Summary

In this assignment, you installed a virtualized Ubuntu distribution of the Linux operating system using Oracle VirtualBox. The objective was to learn how to load and operate an OS in a virtualized environment, understand the usefulness of a virtualized OS, work with Linux in a virtualized environment, and understand the difference between NAT and direct network connections. You followed a series of steps to create a virtual machine, install Ubuntu from an ISO file, update the installation, configure the network settings, and perform network scans using nmap. Additionally, you experimented with various Linux commands and optionally installed and used SSH for secure remote access.

### Commands used in the assignment

- `sudo apt-get update && sudo apt-get upgrade -y`: Updates the Ubuntu system.
- `sudo apt install net-tools`: Installs the net-tools package.
- `ifconfig`: Displays network interface information.
- `nmap 10.81.104.0/24`: Scans the lab network.
- `nmap 10.81.104.0/24 -p 1-1024`: Scans for open ports on the network.
- `nmap -O 10.81.104.0/24`: Attempts to scan for OS versions of devices (requires root privileges).
- `grep -i up scan.txt`: Searches for the pattern "up" in the scan.txt file.
- `mkdir fun`: Creates a directory named "fun".
- `mkdir fun\stuff`: Creates a subdirectory "stuff" inside "fun".
- `cd fun`: Changes the directory to "fun".
- `ls`: Lists the contents of the current directory.
- `cd stuff`: Changes the directory to "stuff".
- `cd ..`: Moves up one level in the directory structure.
- `rmdir stuff`: Removes the "stuff" directory.
- `cd ~`: Changes the directory to the user's home directory.
- `echo hello, my name is puddintane >> new.txt`: Appends the text to a file named "new.txt".
- `nano new.txt`: Opens the new.txt file in the nano text editor.
- `hostname`: Displays the hostname of the system.
- `touch somefile.txt`: Creates an empty file named "somefile.txt".

### SSH server setup and remote access

- `sudo apt-get install openssh-server`: Installs OpenSSH server on the Ubuntu VM.
- `sudo systemctl start ssh`: Starts the SSH service on the Ubuntu VM.
- `sudo systemctl status ssh`: Displays the status of the SSH service.

![Remote Access VM](Remote_accessVM.png)
![screenshot](Screenshot_2023-05-08_031428.png)
![screenshot](Screenshot_2023-05-08_031443.png)
![screenshot](Screenshot_2023-05-08_031456.png)
![screenshot](Screenshot_2023-05-08_031506.png)
![screenshot](Screenshot_2023-05-08_033321.png)
