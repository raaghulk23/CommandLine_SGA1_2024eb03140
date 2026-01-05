You have been asked to understand how Linux manages files using links and disk usage information.As part of your role, you will perform the following operations within your own user space.

1. File Creation
Create a file named sample_data.txt in your home directory and add some sample text to it.
## Commands used: 
pwd
vi sample_data.txt
## Output Screenshot:
Command Line SGA1/Question1/3a.png
## Explanation:
pwd shows that the current directory is home. Used vi command to create sample_data file and added some text. 

2. Hard Link Creation
Create a hard link to sample_data.txt named sample_hard.txt.
## Commands used: 
ln sample_data.txt sample_hard.txt
## Output Screenshot:
Command Line SGA1/Question1/3b.png
## Explanation:
Created a hard link using the ln command.

3. Symbolic Link Creation
Create a symbolic (soft) link to sample_data.txt named sample_soft.txt.
## Commands used: 
ln -s sample_data.txt sample_soft.txt
## Output Screenshot:
Command Line SGA1/Question1/3c.png
## Explanation:
Created a soft link using the ln -s command.

4. Inode Verification
Display the inode numbers of sample_data.txt, sample_hard.txt, and sample_soft.txt.
## Commands used: 
ls -i sample_data.txt sample_hard.txt sample_soft.txt
## Output Screenshot:
Command Line SGA1/Question1/3d.png
## Explanation:
Above ls -i shows the inode numbers of sample and its link files.

5. Inode Analysis
Identify which files share the same inode number and briefly explain the reason.
## Commands used: 
ls -li
## Output Screenshot:
Command Line SGA1/Question1/3e.png
## Explanation:
ls -li command shows the hard link and actual file has the same inode number because its not a new copy of the file. 

6. File Metadata Inspection
Display detailed file information (permissions, ownership, size, timestamps) of sample_data.txt.
## Commands used: 
ls -l sample_data.txt
## Output Screenshot:
Command Line SGA1/Question1/3f.png
## Explanation:
shows all details of the sample_data.txt file.

7. Disk Usage Check
Display the disk usage of your home directory in a human-readable format.
## Commands used:
du -sh ~
du -h
## Output Screenshot:
Command Line SGA1/Question1/3g.png
## Explanation:
du -sh ~ shows the disk usage of the home directory

8. File Size Overview
Display the size of each file present in your home directory in a human-readable format.
## Commands used:
ls -lh ~
## Output Screenshot:
Command Line SGA1/Question1/3h.png
## Explanation:
This command shows the details of each file in the home directory

9. Link Deletion Test
Delete the symbolic link sample_soft.txt and verify that the original file sample_data.txt is unaffected.
## Commands used: 
rm sample_soft.txt
## Output Screenshot:
Command Line SGA1/Question1/3i.png
## Explanation:
Soft link is deleted using the rm command.

10. Disk Utility Demonstration
Demonstrate the usage of du and df commands using various useful options and briefly explain the output.
## Commands used: 
df -h
df -T
df -a
df -i
du -sh ~
du -h
du -a
du -c
## Output Screenshot:
Command Line SGA1/Question1/3j1.png
Command Line SGA1/Question1/3j2.png
## Explanation:
du -sh ~ shows the total disk usage in the home directory, -h shows the current directory disk usage in human readable format, -a shows the size of every file and directory, -c shows details along with a grand total.

df -h shows the amount of space available in human readable format, -a shows for all file systems including dummy, -i displays inode information, -T adds a flag to show the file type.