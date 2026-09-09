# linux-commands
🐧 Linux Commands | Beginner to Advanced | Examples, Exercises &amp; Real-World Usage

# Linux Commands

A structured collection of **Linux commands, examples, explanations, and practical exercises** for beginners and developers.

This repository is organized topic-by-topic so that Linux commands can be learned and referenced quickly.

---

## Repository Structure

```text
linux-commands/
│
├── 01-file-directory/       # File and directory navigation
├── 02-file-operations/      # Copy, move, remove, links
├── 03-file-content/         # Read and inspect file contents
├── 04-search/               # Find files and search text
├── 05-permissions/          # Linux permissions and ownership
├── 06-users-groups/         # Users and groups
├── 07-processes/            # Process management
├── 08-networking/           # Networking commands
├── 09-disk-storage/         # Disk and storage management
├── 10-archives/             # Archive and compression commands
├── 11-text-processing/      # Text processing commands
├── 12-shell/                # Shell and environment commands
├── 13-system/               # System information and management
├── 14-package-management/   # Package management
├── 15-git/                  # Git commands and exercises
│
├── exercises/               # Practical Linux exercises
│
└── README.md
```

---

# Linux Commands Quick Reference

## 1. File & Directory

| Command           | Description                    |
| ----------------- | ------------------------------ |
| `pwd`             | Show current directory         |
| `ls`              | List files and directories     |
| `ls -l`           | List with detailed information |
| `ls -a`           | Show hidden files              |
| `ls -lh`          | Show human-readable sizes      |
| `cd <dir>`        | Change directory               |
| `cd ..`           | Go to parent directory         |
| `cd ~`            | Go to home directory           |
| `mkdir <dir>`     | Create directory               |
| `mkdir -p <path>` | Create nested directories      |
| `touch <file>`    | Create empty file              |

---

## 2. File Operations

| Command               | Description                  |
| --------------------- | ---------------------------- |
| `cp <src> <dest>`     | Copy a file                  |
| `cp -r <src> <dest>`  | Copy directory recursively   |
| `mv <src> <dest>`     | Move or rename               |
| `rm <file>`           | Remove a file                |
| `rm -r <dir>`         | Remove directory recursively |
| `rm -i <file>`        | Ask before removing          |
| `rmdir <dir>`         | Remove empty directory       |
| `ln <file> <link>`    | Create hard link             |
| `ln -s <file> <link>` | Create symbolic link         |

---

## 3. File Content

| Command          | Description                |
| ---------------- | -------------------------- |
| `cat <file>`     | Display file content       |
| `less <file>`    | View file page by page     |
| `more <file>`    | View file page by page     |
| `head <file>`    | Show first lines           |
| `tail <file>`    | Show last lines            |
| `tail -f <file>` | Follow file changes        |
| `nl <file>`      | Display lines with numbers |
| `file <file>`    | Identify file type         |
| `stat <file>`    | Show file information      |

---

## 4. Search

| Command                   | Description                       |
| ------------------------- | --------------------------------- |
| `find <path>`             | Search for files/directories      |
| `locate <name>`           | Quickly search file paths         |
| `grep <pattern> <file>`   | Search text in a file             |
| `grep -r <pattern> <dir>` | Search recursively                |
| `which <command>`         | Show command location             |
| `whereis <command>`       | Locate binary, source, and manual |

---

## 5. Permissions

| Command                | Description                  |
| ---------------------- | ---------------------------- |
| `ls -l`                | View permissions             |
| `chmod <mode> <file>`  | Change permissions           |
| `chmod +x <file>`      | Add execute permission       |
| `chown <user> <file>`  | Change file owner            |
| `chgrp <group> <file>` | Change group ownership       |
| `umask`                | Show default permission mask |

### Permission Types

```text
r = read
w = write
x = execute
```

Example:

```bash
chmod 755 script.sh
```

---

## 6. Users & Groups

| Command    | Description                              |
| ---------- | ---------------------------------------- |
| `whoami`   | Show current username                    |
| `id`       | Show user and group IDs                  |
| `who`      | Show logged-in users                     |
| `w`        | Show logged-in users and activity        |
| `groups`   | Show user's groups                       |
| `passwd`   | Change password                          |
| `useradd`  | Create user                              |
| `usermod`  | Modify user                              |
| `userdel`  | Delete user                              |
| `groupadd` | Create group                             |
| `groupdel` | Delete group                             |
| `sudo`     | Execute command with elevated privileges |

---

## 7. Processes

| Command         | Description                 |
| --------------- | --------------------------- |
| `ps`            | Show processes              |
| `ps aux`        | Show detailed process list  |
| `top`           | Monitor processes           |
| `htop`          | Interactive process monitor |
| `pgrep`         | Find process IDs            |
| `kill <PID>`    | Send signal to process      |
| `kill -9 <PID>` | Force terminate process     |
| `pkill <name>`  | Kill process by name        |
| `jobs`          | Show shell jobs             |
| `bg`            | Resume job in background    |
| `fg`            | Bring job to foreground     |
| `nohup`         | Run command after logout    |

---

## 8. Networking

| Command             | Description                           |
| ------------------- | ------------------------------------- |
| `ip addr`           | Show network interfaces and addresses |
| `ip link`           | Show network interfaces               |
| `ping <host>`       | Test network connectivity             |
| `curl <url>`        | Transfer data from a URL              |
| `wget <url>`        | Download files                        |
| `ss`                | Show network sockets                  |
| `ssh <user>@<host>` | Connect to remote system              |
| `scp <src> <dest>`  | Securely copy files                   |
| `dig <domain>`      | Query DNS information                 |
| `nslookup <domain>` | Query DNS information                 |
| `traceroute <host>` | Trace network path                    |

---

## 9. Disk & Storage

| Command        | Description                |
| -------------- | -------------------------- |
| `df -h`        | Show filesystem disk usage |
| `du -sh <dir>` | Show directory size        |
| `du -h`        | Show file/directory sizes  |
| `lsblk`        | List block devices         |
| `mount`        | Mount filesystem           |
| `umount`       | Unmount filesystem         |
| `fdisk`        | Manage disk partitions     |
| `free -h`      | Show memory usage          |
| `sync`         | Flush filesystem buffers   |

---

## 10. Archives & Compression

| Command    | Description                    |
| ---------- | ------------------------------ |
| `tar -cf`  | Create tar archive             |
| `tar -xf`  | Extract tar archive            |
| `tar -czf` | Create gzip-compressed archive |
| `tar -xzf` | Extract gzip archive           |
| `gzip`     | Compress file                  |
| `gunzip`   | Decompress gzip file           |
| `zip`      | Create ZIP archive             |
| `unzip`    | Extract ZIP archive            |

---

## 11. Text Processing

| Command | Description                    |
| ------- | ------------------------------ |
| `grep`  | Search text                    |
| `sed`   | Stream editor                  |
| `awk`   | Process structured text        |
| `cut`   | Extract columns/fields         |
| `sort`  | Sort lines                     |
| `uniq`  | Remove/count duplicate lines   |
| `wc`    | Count lines, words, and bytes  |
| `head`  | Show beginning of file         |
| `tail`  | Show end of file               |
| `tr`    | Translate or delete characters |

---

## 12. Shell

| Command   | Description                   |
| --------- | ----------------------------- |
| `echo`    | Print text                    |
| `history` | Show command history          |
| `alias`   | Create command shortcuts      |
| `export`  | Set environment variable      |
| `env`     | Show environment variables    |
| `source`  | Execute file in current shell |
| `which`   | Find executable location      |
| `man`     | Open command manual           |
| `type`    | Show command type             |

---

## 13. System

| Command    | Description                    |
| ---------- | ------------------------------ |
| `uname -a` | Show system information        |
| `hostname` | Show system hostname           |
| `date`     | Show current date/time         |
| `uptime`   | Show system uptime             |
| `whoami`   | Show current user              |
| `who`      | Show logged-in users           |
| `id`       | Show user identity information |
| `reboot`   | Restart the system             |
| `shutdown` | Shut down or restart system    |

---

## 14. Package Management

### APT

| Command                 | Description                      |
| ----------------------- | -------------------------------- |
| `apt update`            | Update package information       |
| `apt upgrade`           | Upgrade installed packages       |
| `apt install <package>` | Install package                  |
| `apt remove <package>`  | Remove package                   |
| `apt purge <package>`   | Remove package and configuration |
| `apt search <package>`  | Search for packages              |
| `apt show <package>`    | Show package information         |
| `apt autoremove`        | Remove unused packages           |

### DPKG

| Command                 | Description             |
| ----------------------- | ----------------------- |
| `dpkg -i <package.deb>` | Install `.deb` package  |
| `dpkg -l`               | List installed packages |
| `dpkg -s <package>`     | Show package status     |
| `dpkg -r <package>`     | Remove package          |

### Snap

| Command                  | Description          |
| ------------------------ | -------------------- |
| `snap list`              | List installed snaps |
| `snap install <package>` | Install snap         |
| `snap remove <package>`  | Remove snap          |
| `snap refresh`           | Update snaps         |

---

# 15. Git

| Command                 | Description                     |
| ----------------------- | ------------------------------- |
| `git init`              | Initialize repository           |
| `git clone <url>`       | Clone repository                |
| `git status`            | Show repository status          |
| `git add <file>`        | Stage file                      |
| `git add .`             | Stage current directory changes |
| `git commit -m "msg"`   | Create commit                   |
| `git push`              | Push commits                    |
| `git pull`              | Fetch and integrate changes     |
| `git fetch`             | Download remote changes         |
| `git branch`            | List branches                   |
| `git switch <branch>`   | Switch branch                   |
| `git switch -c <name>`  | Create and switch branch        |
| `git checkout <branch>` | Switch branch                   |
| `git merge <branch>`    | Merge branch                    |
| `git log`               | Show commit history             |
| `git log --oneline`     | Show compact history            |
| `git diff`              | Show unstaged changes           |
| `git diff --staged`     | Show staged changes             |
| `git remote -v`         | Show remote repositories        |
| `git reset`             | Reset staging/commits           |
| `git restore`           | Restore file changes            |
| `git stash`             | Temporarily save changes        |
| `git stash pop`         | Restore latest stash            |
| `git tag`               | Manage tags                     |
| `git show`              | Show commit/tag details         |
| `git rm`                | Remove tracked file             |
| `git mv`                | Rename/move tracked file        |

---

# Common Linux Operators

| Operator | Description                           |   |                                    |
| -------- | ------------------------------------- | - | ---------------------------------- |
| `>`      | Redirect output and overwrite         |   |                                    |
| `>>`     | Redirect output and append            |   |                                    |
| `<`      | Redirect input                        |   |                                    |
| `\|`     | Pipe output to another command        |   |                                    |
| `&&`     | Run next command if previous succeeds |   |                                    |
| `        |                                       | ` | Run next command if previous fails |
| `;`      | Run commands sequentially             |   |                                    |
| `&`      | Run command in background             |   |                                    |

### Examples

```bash
ls -l > files.txt
```

```bash
cat file.txt | grep "error"
```

```bash
mkdir project && cd project
```

---

# Useful Shortcuts

| Shortcut   | Description              |
| ---------- | ------------------------ |
| `Ctrl + C` | Stop running command     |
| `Ctrl + D` | Exit shell / send EOF    |
| `Ctrl + Z` | Suspend running process  |
| `Ctrl + L` | Clear terminal           |
| `Ctrl + R` | Search command history   |
| `Tab`      | Auto-complete            |
| `↑` / `↓`  | Navigate command history |

---

# Getting Help

```bash
man <command>
```

```bash
<command> --help
```

```bash
info <command>
```

Examples:

```bash
man ls
```

```bash
grep --help
```

---

# Recommended Learning Order

Learn the commands in this order:

```text
01. File & Directory
        ↓
02. File Operations
        ↓
03. File Content
        ↓
04. Search
        ↓
05. Permissions
        ↓
06. Users & Groups
        ↓
07. Processes
        ↓
08. Networking
        ↓
09. Disk & Storage
        ↓
10. Archives
        ↓
11. Text Processing
        ↓
12. Shell
        ↓
13. System
        ↓
14. Package Management
        ↓
15. Git
```

---

# Exercises

The `exercises/` directory contains practical tasks to reinforce the commands.

```text
exercises/
├── 01-file-directory/
├── 02-file-operations/
├── 03-file-content/
├── 04-search/
├── 05-permissions/
├── 06-users-groups/
├── 07-processes/
├── 08-networking/
├── 09-disk-storage/
├── 10-archives/
├── 11-text-processing/
├── 12-shell/
├── 13-system/
├── 14-package-management/
└── 15-git/
```

Use the exercises after studying each topic.

---

# Quick Daily Linux Reference

The commands most commonly used in everyday Linux work are:

```bash
pwd
ls
cd
mkdir
touch
cp
mv
rm
cat
less
head
tail
grep
find
chmod
chown
ps
top
kill
df
du
free
ip
ping
curl
ssh
tar
grep
sed
awk
echo
export
man
sudo
```

For Git:

```bash
git status
git add .
git commit -m "message"
git pull
git push
git branch
git switch
git merge
git log --oneline
git diff
git stash
```

---

# Purpose of This Repository

This repository is intended to serve as:

* 📚 Linux learning notes
* ⚡ Quick command reference
* 💻 Daily Linux reference
* 🧪 Practical exercise collection
* 🚀 Developer/Linux interview preparation

The individual topic folders contain **detailed command documentation**, while this `README.md` provides a **quick reference**.

