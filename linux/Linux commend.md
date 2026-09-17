```
mv /home/c/myfile/text.txt /home/f/ (file move example)
cp /home/c/myfile/text.txt /home/f/ (file copy example)
top (show most consuming possessing)
ps (show all possessing)
ps -a (show all possessing in details)
kill 2557 (kill a possessing with Possess ID)
sudo su (be regular user to root user)
apt install vim (example of installing a software)
Commend To Refresh Application Menu list: update-desktop-database ~/.local/share/applications
Giveing A File Executeing Permission: chmod +x your_file_name.run
Run The Executeable file: sudo ./your_file_name.run
Xampp Commands: sudo /opt/lampp/lampp start, stop, restart, startapache, startmysql
Recursively delete a directory and its files: rm -rf directory/
```


### Current path ###
```
pwd
```

### List path ###
```
ls
```

### Folder creation ###
```
mkdir [folder name]
```

### Show all executed command ###
```
history
```

### Recursive listing ###
```
ls -R
```

## Enable the Magic SysRq Key ##
```
echo 'kernel.sysrq=1' | sudo tee /etc/sysctl.d/99-sysrq.conf
sudo sysctl -p /etc/sysctl.d/99-sysrq.conf
```

### Emergency REISUB Reboot (Safe Kernel Reboot) ###
```
Alt + SysRq + R
Alt + SysRq + E
Alt + SysRq + I
Alt + SysRq + S
Alt + SysRq + U
Alt + SysRq + B

```

### SysRq Commands ###

```
b - Reboot - Immediately reboots the system without syncing or unmounting
c - Crash - Forces a kernel panic (for crash dump testing)
d - Show locks - Dumps kernel locks held by tasks
e - Terminate - Sends SIGTERM to all processes except init
f - OOM-Killer - Forces the out-of-memory killer to run
g - Unused - No function assigned
h - Help - Prints SysRq help to the kernel log
i - Kill - Sends SIGKILL to all processes except init
j - Thaw - Thaws frozen processes (freezer/ftrace)
k - Kill TTY - Kills all processes on the current virtual terminal
l - Show backtrace - Dumps stack traces of all active CPUs
m - Memory info - Dumps memory info to logs (like /proc/meminfo)
n - Reset nice - Resets all process priorities (nice value to 0)
o - Power off - Powers off the machine (if supported)
p - Show registers - Dumps CPU registers to logs
q - Show Qdisc - Dumps network queue information
r - Keyboard raw mode - Switches keyboard from X to raw mode
s - Sync - Flushes all disk caches to disk
t - Show tasks - Shows all running processes (process table)
u - Unmount - Remounts all filesystems read-only
v - Show virtual memory - Dumps virtual memory info
w - Show blocked tasks - Lists tasks stuck in uninterruptible sleep
x - Show interrupts - Dumps interrupt info
y - Show CPU core data - Dumps per-CPU core details
z - Show pagetable - Dumps current pagetable info
```

### Enable USB File Transfer for linux ###

```
sudo apt update
sudo apt install mtp-tools gvfs-backends gvfs-fuse
```

### Create New User
```
adduser [user name]
```

### Give User The Root Privileges

```
usermod -aG sudo [user name]
```

### Copy Root User SSH To New User So You Can Log In To The Machine Using That Other User

```
cp -r --preserve=mode /root/.ssh /home/[user name]
```
