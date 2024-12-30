# Linux-Forensics
A Quick guide to Linux Forensics 

# Linux Forensics Cheat Sheet

This **Linux Forensics Cheat Sheet** provides a categorized overview of key files and commands for gathering system information, examining evidence, and analyzing system logs. It is a handy reference for digital forensic investigations and incident response.

---

## Table of Contents
1. [System and OS Information](#system-and-os-information)
2. [System Configuration](#system-configuration)
3. [Persistence Mechanisms](#persistence-mechanisms)
4. [Evidence of Execution](#evidence-of-execution)
5. [Log Files](#log-files)

---

## System and OS Information
- **OS Release Information**: `/etc/os-release`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **User Accounts Information**: `/etc/passwd`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **User Group Information**: `/etc/group`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **Sudoers List**: `/etc/sudoers`
  - Requires root permission for access. Use `cat`, `vim`, or a text editor.

- **Login Information**: `/var/log/wtmp`
  - Can be read using the `last` utility.

- **Authentication Logs**: `/var/log/auth.log`
  - Can be read using `cat`, `vim`, or any text editor/viewer.
  - Useful for filtering failed login attempts and other security events.

---

## System Configuration
- **Hostname**: `/etc/hostname`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **Timezone Information**: `/etc/timezone`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **Network Interfaces**: `/etc/network/interfaces`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **DNS Information**: `/etc/resolv.conf`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

---

## Persistence Mechanisms
- **Cron Jobs**: `/etc/crontab`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **Services**: `/etc/init.d/`
  - Registered services are present in this directory.

- **Bash Shell Startup Scripts**: `/home/<user>/.bashrc`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **System-wide Configurations**: `/etc/bash.bashrc` or `/etc/profile`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

---

## Evidence of Execution
- **Authentication Logs**: `/var/log/auth.log`
  - Use `grep 'COMMAND' /var/log/auth.log` to filter results.

- **Bash History**: `/home/<user>/.bash_history`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

- **Vim History**: `/home/<user>/.viminfo`
  - Can be read using `cat`, `vim`, or any text editor/viewer.

---

## Log Files
- **System Logs**: `/var/log/syslog`
  - Can be read using `cat`, `vim`, or any text editor/viewer.
  - Useful for analyzing system activity and events.

- **Application Logs**: `/var/log`
  - Location depends on the application configuration.

---

## Contributions
Feel free to suggest improvements or submit issues and pull requests to enhance this resource.
