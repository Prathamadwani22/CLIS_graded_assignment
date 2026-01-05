# Question 1

### 1. System Uptime Verification

```
$ uptime
```
- This command displays how long the system has been running since the last boot.

![System Uptime Verification](Snapshots/task_1.png)

---
### 2. User Process Listing

```
$ ps -u $(whoami)
```
- `ps -u` lists all processes currently running under the logged-in user account.

![User Process Listing](Snapshots/task_2.png)

---
### 3. CPU Usage Analysis

```
$ top -o cpu
```
- This lists user processes sorted by CPU usage, with the highest CPU-consuming process shown first.

![CPU Usage Analysis](Snapshots/task_3.png)

---
### 4. Background Process Execution

```
$ sleep 300 & jobs
```
- `sleep 300 &` starts a background process, and `jobs` confirms that the background job is running.

![Background Process Execution](Snapshots/task_4.png)

---
### 5. Process Priority Management

```
$ renice 5 -p <PID>
```

```
$ ps -o pid,ni,command -p <PID>
```
- `renice` changes the priority (niceness) of the specified process, and `ps` confirms the updated niceness value.

![Process Priority Management](Snapshots/task_5.png)

---
### 6. Memory Usage Monitoring

```
$ free -h
```
- `free -h` displays system memory usage in a human-readable format, including used and available memory.

![Memory Usage Monitoring](Snapshots/task_6.png)

---
### 7. Disk Space Inspection

```
$ df -h ~
```
- This command shows disk space usage of the filesystem where the home directory resides.

![Disk Space Inspection](Snapshots/task_7.png)

---
### 8. Shell Identification

```
$ echo $SHELL
```
- This outputs the name and path of the shell currently in use.

![Shell Identification](Snapshots/task_8.png)

---
### 9. Output Redirection

```
$ uname -a > system_report.txt
```
- This redirects system information output into the file `system_report.txt`.

![Output Redirection](Snapshots/task_9.png)
[system_report.txt](system_report.txt)

---
### 10. Disk Usage Visualization

```
$ ncdu ~
```
- `ncdu` provides an interactive, text-based visualization of disk usage within the home directory, showing space consumed by files and directories.

![Disk Usage Visualization](Snapshots/task_10.png)