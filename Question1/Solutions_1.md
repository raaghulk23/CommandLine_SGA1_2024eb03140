You have just joined IxD Systems as a junior systems engineer. On your first day, the Linux administrator asks you to perform a basic environment verification on the lab machine using your own login account.

### 1. User Identity Verification
Display your currently logged-in username and all groups your user account belongs to.
Your name or login ID must appear in the output.
###### Commands used: 
whoami
groups 
id
###### Output Screenshot:
Command Line SGA1/Question1/1a.png
###### Explanation:
whoami displays the current user loggedin.
groups shows the name of the groups for the user.
id shows the ID of the user.

### 2. Workspace Validation
Display the current working directory and list all files and directories in that location using long format listing.
###### Commands used: 
pwd
ls -l
###### Output Screenshot:
Command Line SGA1/Question1/1b.png
###### Explanation:
pwd shows the current working directory
ls -l shows the contents of the current working directory


### 3. Environment Confirmation File
Create a file named user_info.txt and write the line:
&quot;Linux user environment verified&quot;
###### Commands used: 
vi user_info.txt
###### Output Screenshot:
Command Line SGA1/Question1/1c.png
###### Explanation:
vi command is used to create and open a file using the name given


### 4. File Integrity Check
Display the number of characters present in user_info.txt.
###### Commands used: 
wc -m user_info.txt
###### Output Screenshot:
Command Line SGA1/Question1/1d.png
###### Explanation:
wc command counts the number of characters in a file.


### 5. Learning the Tools
Access the manual page of the mkdir command. Identify one useful option and briefly explain what it does.
###### Commands used: 
man mkdir
###### Output Screenshot:
Command Line SGA1/Question1/1e.png
###### Explanation:
man mkdir has given the details and all the options for the mkdir command.


### 6. Home Directory Inspection
List the contents of your home directory sorted alphabetically.
###### Commands used: 
pwd
ls ~
ls -l ~
###### Output Screenshot:
Command Line SGA1/Question1/1f.png
###### Explanation:
ls ~ shows the contents of the user's home directory. 
ls -l ~ command shows the long listing format.


### 7. Log Investigation
Search for the word &quot;admin&quot; inside a file named log.txt and display only the matching lines.
###### Commands used: 
ls
vi log.txt
grep "admin" log.txt
###### Output Screenshot:
Command Line SGA1/Question1/1g.png
###### Explanation:
vi log.txt command created a file log.txt. And i added some sample text containing admin word in some of the lines.
grep command showed the lines containing the word "admin".


### 8. System Information Check
Display the Linux kernel version currently running.
###### Commands used: 
uname -r
###### Output Screenshot:
Command Line SGA1/Question1/1h.png
###### Explanation:
Above input shows the kernel release. 


### 9. Network Connectivity Test
Verify network connectivity by sending ICMP packets to www.google.com.
###### Commands used: 
ping www.google.com
###### Output Screenshot:
Command Line SGA1/Question1/1i.png
###### Explanation:
ping command is used to test the connectivity between the server and my computer.


### 10. System Health Awareness
Display the command used to check system uptime and briefly explain its output (uptime duration, number of users, load average).
###### Commands used: 
uptime
###### Output Screenshot:
Command Line SGA1/Question1/1j.png
###### Explanation:
this command shows how long my computer has been up and running. 
