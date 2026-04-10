# Linux Fundamentals: Technical Reference & Quiz Summary

## Core Command Summary

### File Management
* **rm**: Removes files. Requires only one argument (the target). 
* **rm -r**: Recursive removal, required to delete directories and their contents.
* **tail**: Displays the end of a file. Use `tail -n 5` or `tail -5` for the last five lines.
* **echo**: Prints text or shell variables to the standard output.

### Package Management (Debian/Ubuntu)
* **apt-get update**: Synchronizes the local package index with the remote repositories. Must be run before installing new packages.
* **apt-get upgrade**: Installs the newest versions of all packages currently installed.
* **apt-get purge**: Removes a package along with all its configuration files.
* **apt-get remove**: Removes the package but leaves configuration files intact.

### Process & User Administration
* **ps -e**: Displays every process currently running on the system.
* **ps**: By default, shows only processes attached to the current terminal. Does not require root privileges.
* **passwd [user]**: When run by root, allows changing any user's password without knowing the current one.
* **passwd -S**: Displays the status of a user's password (e.g., locked, set, or expired).

### Networking & I/O
* **ifconfig**: Used to view and configure network interface parameters (IP address, Netmask, etc.).
* **ping**: Uses ICMP Echo Requests and IP addresses to test host reachability and latency.
* **Redirection (>)**: Redirects Standard Output (STDOUT) to a file, overwriting existing content.
* **Regex ($)**: The dollar sign anchor matches the end of a line (e.g., `grep 'test$'` finds lines ending in "test").

---

## Quiz Review

| Question | Answer |
| :--- | :--- |
| Does the `rm` command require at least two arguments? | **False** |
| Which option allows `rm` to delete directories? | **-r** |
| Which command displays network configuration? | **ifconfig** |
| Which command returns only lines ending with "test"? | **grep 'test$' file.txt** |
| Which command displays every running process? | **ps -e** |
| Does the `ps` command require administrative access? | **False** |
| Which command installs available package updates? | **apt-get upgrade** |
| Which command deletes a package and its config files? | **apt-get purge** |
| Which command should be executed before installing a package? | **apt-get update** |
| Which command prints output to the terminal? | **echo** |
| The `>` character is used for which file descriptor? | **STDOUT** |
| Which command shows the last five lines of a file? | **tail -n 5 file.txt** |
| Can the root user change the password of any user? | **True** |
| Which flag is used to view password status information? | **-S** |
| Does `ping` use IP addresses to identify computers? | **True** |
