### 1. Project Workspace Setup
Create a directory named documents inside your home directory. This directory will store your project-related files.
#### Commands used: 
mkdir documents
#### Output Screenshot:
Command Line SGA1/Question1/2a.png
#### Explanation:
this command created a new directory named documents

### 2. File Creation
Navigate into the documents directory and create a file named plan.txt.
#### Commands used: 
cd documents
touch plan.txt
#### Output Screenshot:
Command Line SGA1/Question1/2b.png
#### Explanation:
navigated inside the directory using the cd command and created a file using the touch command.


### 3. Content Addition
Write some sample text of your choice into the plan.txt file. The content can be a short project note or reminder.
#### Commands used: 
vi plan.txt
#### Output Screenshot:
Command Line SGA1/Question1/2c.png
#### Explanation:
Opened the sample file and added contents using the vi command.

### 4. File Metadata Verification
Display the permissions and ownership details of the plan.txt file. Ensure your username appears in the output.
#### Commands used: 
ls -l plan.txt
#### Output Screenshot:
Command Line SGA1/Question1/2d.png
#### Explanation:
ls -l command shows the permissions and ownership details.

### 5. File Duplication
Create a copy of plan.txt and name it plan_copy.txt.
#### Commands used: 
cp plan.txt plan_copy.txt 
#### Output Screenshot:
Command Line SGA1/Question1/2e1.png
Command Line SGA1/Question1/2e2.png
#### Explanation:
Copied the file using the cp command.

### 6. Directory Renaming
Rename the documents directory to project_documents to reflect the project scope more clearly.
#### Commands used: 
mv documents project_documents
#### Output Screenshot:
Command Line SGA1/Question1/2f.png
#### Explanation:
Renamed the file using the mv command.

### 7. Archival Structure
Inside the project_documents directory, create a subdirectory named archive.
#### Commands used: 
mkdir project_documents/archive
#### Output Screenshot:
Command Line SGA1/Question1/2g.png
#### Explanation:
created a subdirectory using the above mentioned mkdir command.

### 8. File Organization
Move plan_copy.txt into the archive subdirectory.
#### Commands used: 
mv plan_copy.txt archive/
#### Output Screenshot:
Command Line SGA1/Question1/2h.png
#### Explanation:
moved the file to the archive directory using the mv command. 

### 9. Recursive Listing
List all files and subdirectories inside project_documents recursively so that the complete directory structure is visible.
#### Commands used: 
ls -R project_documents
#### Output Screenshot:
Command Line SGA1/Question1/2i.png
#### Explanation:
This command showed the contents of the directory and its subdirectories.

### 10. Path Verification
Display the absolute path of the plan_copy.txt file after it has been moved to the archive directory.
#### Commands used: 
realpath project_documents/archive/plan_copy.txt
#### Output Screenshot:
Command Line SGA1/Question1/2j.png
#### Explanation:
realpath command shows the absolute path of the plan_copy.txt file.