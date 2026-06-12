# Linux Cheat Sheet

## 1. File System Navigation
- `pwd` — Print current working directory.
- `ls` — List files and folders in the current directory.
  - `ls -l` — Long format listing with file details.
  - `ls -a` — Show hidden files (those beginning with `.`).
  - `ls -lh` — Human-readable file sizes.
- `cd <directory>` — Change directory.
  - `cd ..` — Go up one directory.
  - `cd ~` or `cd` — Go to the home directory.
  - `cd /` — Go to the root directory.
- `tree` — Display directory structure as a tree (install if missing).
- `find . -name "*.txt"` — Search for files by name.

## 2. File & Directory Permissions
- `ls -l` — View permissions, owner, and group.
  - Example: `-rw-r--r-- 1 user group  512 Jun 12 file.txt`
- `chmod <mode> <file>` — Change file or directory permissions.
  - `chmod 755 file.sh` — Owner can read/write/execute; others can read/execute.
  - `chmod 644 file.txt` — Owner read/write; others read-only.
  - `chmod +x script.sh` — Add execute permission.
- `chown <user>:<group> <file>` — Change file owner and group.
  - `chown kali:kali file.txt`
  - `chown root:root /usr/local/bin/tool`
- `stat <file>` — Show detailed file information.

## 3. Package Management
### Debian/Ubuntu package tools
- `sudo apt update` — Refresh package list.
- `sudo apt upgrade` — Upgrade installed packages.
- `sudo apt install <package>` — Install a package.
- `sudo apt remove <package>` — Remove a package.
- `sudo apt purge <package>` — Remove package and configuration files.
- `sudo apt autoremove` — Remove unused packages.

### Low-level package management
- `dpkg -i <file.deb>` — Install a `.deb` package file.
- `dpkg -r <package>` — Remove an installed package.
- `dpkg -l | grep <name>` — List installed packages.
- `dpkg -s <package>` — Show package status and info.

## 4. Networking Commands
- `ifconfig` — Show network interface configuration.
  - Use `ip a` on newer systems as a modern replacement.
- `ping <host>` — Send ICMP echo requests to test connectivity.
  - Example: `ping 192.168.56.101`
- `netstat -tulnp` — Show active listening ports and services.
- `ss -tuln` — Modern replacement for `netstat`.
- `traceroute <host>` — Trace network route to a host.
- `curl -I <url>` — Show HTTP headers from a website.
- `wget <url>` — Download files from the web.

## 5. Basic File Operations
- `cat file.txt` — Display file contents.
- `less file.txt` — View file contents page by page.
- `cp source dest` — Copy files or directories.
  - `cp -r folder1 folder2` — Copy directories recursively.
- `mv source dest` — Move or rename files/directories.
- `rm file.txt` — Delete a file.
  - `rm -r folder` — Delete directory recursively.
  - `rm -f file.txt` — Force delete without confirmation.
- `mkdir folder` — Create a new directory.
- `rmdir folder` — Remove an empty directory.

## 6. Useful Linux Tips
- `sudo <command>` — Run a command as root.
- `whoami` — Show current user.
- `uname -a` — Display system and kernel information.
- `history` — Show recently used commands.
- `clear` — Clear the terminal screen.

## 7. Linux Commands Cheat Sheet Summary
| Task | Command |
| --- | --- |
| Current directory | `pwd` |
| List files | `ls`, `ls -la` |
| Change directory | `cd <dir>` |
| Check permissions | `ls -l` |
| Change permissions | `chmod 755 file` |
| Change owner | `chown user:group file` |
| Update packages | `sudo apt update` |
| Install package | `sudo apt install <pkg>` |
| Ping a host | `ping <host>` |
| Show network config | `ifconfig` |
| Trace route | `traceroute <host>` |
| View file | `cat file.txt` |
