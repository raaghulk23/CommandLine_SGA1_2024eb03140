You must perform all operations without making any configuration changes to the system.

These tasks should be executed within your own user account. Since uptime, processes, memory usage,disk usage, and background jobs vary across systems and users, each student’s output will be unique.

### 1. System Uptime Verification
Display the time elapsed since the system was last booted.
#### Commands used: 
uptime -p
#### Output Screenshot:
Command Line SGA1/Question1/4a.png
#### Explanation:
Input command shows how long the system has been up.

### 2. User Process Listing
List all processes currently running under your user account.
#### Commands used: 
ps -u $USER
ps -fu $USER
#### Output Screenshot:
Command Line SGA1/Question1/4b.png
#### Explanation:
ps -u lists all the processes for a user. -fu lists the full format.

### 3. CPU Usage Analysis
Identify the process that is consuming the highest CPU usage among your running processes.
#### Commands used: 
ps aux --sort=%cpu | head -n 1
#### Output Screenshot:
Command Line SGA1/Question1/4c.png
#### Explanation:
displays the processes sorted by the CPU usage.

### 4. Background Process Execution
Start a command in the background and verify that it is running.
#### Commands used: 
sleep 100 &
jobs
kill 5851
#### Output Screenshot:
Command Line SGA1/Question1/4d.png
#### Explanation:
Sleep commmand was used to verify a process. Jobs command was used to that a new job is running in background for sleep. And kill used to destroy the sleep process.

### 5. Process Priority Management
Change the priority (niceness) of one of your running processes and display the updated priority.
#### Commands used: 
sudo renice -10 -p 969
#### Output Screenshot:
Command Line SGA1/Question1/4e.png
#### Explanation:
The above mentioned input command makes it higher priority by reducing the priority value. 

### 6. Memory Usage Monitoring
Display memory usage information in a human-readable format.
#### Commands used: 
free -h
#### Output Screenshot:
Command Line SGA1/Question1/4f.png
#### Explanation:
Shows the free space available in human readable format for the home directory.

### 7. Disk Space Inspection
Display the disk space usage of the filesystem where your home directory resides.
#### Commands used: 
df -h ~
#### Output Screenshot:
Command Line SGA1/Question1/4g.png
#### Explanation:
Shows info about the free space in human readable format in the home directory.

### 8. Shell Identification
Display the name of the shell currently in use.
#### Commands used:
ps -p $$
#### Output Screenshot:
Command Line SGA1/Question1/4h.png
#### Explanation:
Shows info about the current running shell session

### 9. Output Redirection
Redirect the output of a system information command of your choice into a file named system_report.txt.
#### Commands used: 
uname -a > system_report.txt
#### Output Screenshot:
Command Line SGA1/Question1/4i.png
#### Explanation:
This command generates the dummary of the system kernel and hardware info. Saves it and writes them into the file mentioned in the command.

### 10. Disk Usage Visualization
Demonstrate the usage of the ncdu tool using appropriate options and briefly explain what it shows.
#### Commands used: 
ncdu
ncdu /var/log
ncdu -o results.json /home
#### Output Screenshot:
Command Line SGA1/Question1/4j1.png
Command Line SGA1/Question1/4j2.png
Command Line SGA1/Question1/4j3.png
Command Line SGA1/Question1/4j4.png
#### Explanation:
ncdu is used to analyze disk usage and provide details. 
ncdu /var/log analyzes within the /var/log directory.
ncdu -o results.json /home - saves the details of usage of home directory in results.json file