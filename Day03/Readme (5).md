# Day 3: Kali Linux Basics and Windows Hacking

## Introduction

Today's session focused on fundamental commands within the Kali Linux terminal.
## Antivirus Concepts
### Key Antivirus Functions

* **Quarantine Malware:** Antivirus software isolates detected malware to prevent it from infecting or further damaging the system.

### Types of Antivirus Analysis

Antivirus uses two methods for analyzing threats:

* **Static Analysis:**
* **Dynamic Analysis (Runtime Analysis):**
    * Executes the suspicious file in a controlled, isolated environment (sandbox).
    * **Sandbox :** In computing, a sandbox is a secure, isolated environment used for testing and executing code, applications, or programs. 
## Kali Linux Terminal Commands
During the class, I explored and executed several basic commands in the Kali Linux terminal the commands which i used are:
| Command       | Uses                                |Images |
| ------------- | ----------------------------------- |-------|
| `ls`          | Lists directory contents            |<img width="805" height="61" alt="image" src="https://github.com/user-attachments/assets/7a7a5e32-6e38-4a03-a937-8ecf342b69e6" />|
| `cd`          | Changes directory                   |<img width="257" height="97" alt="image" src="https://github.com/user-attachments/assets/f2889d76-59bc-48b5-950f-4db2cfddacf5" />|
| `pwd`         | Shows current directory path        |<img width="252" height="60" alt="image" src="https://github.com/user-attachments/assets/eed05587-9c6e-4a1d-9938-1c3d614c3474" />|
| `mkdir`       | Creates a new directory             |<img width="260" height="105" alt="image" src="https://github.com/user-attachments/assets/054001a9-17eb-4258-aa77-eb6321e9b56c" />|
| `rmdir`       | Deletes an empty directory          |<img width="235" height="162" alt="image" src="https://github.com/user-attachments/assets/06090a09-0ad1-46db-9c91-90ccfb0d3458" />|
| `touch`       | Creates a new empty file            |<img width="260" height="115" alt="image" src="https://github.com/user-attachments/assets/6c7831d1-1d23-448b-900b-c260df7e28da" />|
| `man`         | Opens the manual page for a command |<img width="1901" height="820" alt="image" src="https://github.com/user-attachments/assets/3dd22427-3379-4fe1-9e39-e723db208ae1" /> <img width="176" height="42" alt="image" src="https://github.com/user-attachments/assets/04c9d7ed-1022-4f87-b857-806a9f63d58d" />|
| `echo`        | Prints a message to terminal        |<img width="193" height="62" alt="image" src="https://github.com/user-attachments/assets/8e226830-3c15-4aa6-8f8e-eaafe4ff54da" />|
| `chmod`       | Changes file permissions            |<img width="396" height="131" alt="image" src="https://github.com/user-attachments/assets/dea146ba-5992-4a18-9c17-d82be1052da6" />|
| `clear`       | Clears terminal screen              |Before:<img width="1048" height="897" alt="image" src="https://github.com/user-attachments/assets/84b275cc-ab8b-44bf-baef-d9404e5860c0" /> After:<img width="1057" height="302" alt="image" src="https://github.com/user-attachments/assets/45a1d878-5970-4c74-9047-44c41338ad4e" />|
| `ls -lh`      |Lists directory contents with detailed information |<img width="403" height="67" alt="image" src="https://github.com/user-attachments/assets/3a47ec66-3361-484f-bf48-c44e6cd1be50" />|

### File Permissions:
- **r(Read):** This permission allows user to only read and cant make changes.
- **w(Write):** This permission allows a user to modify, change, or delete the file.
- **x(Execute):** This permission allows user to run the file as a program. 
- Octal Represtation on permissions
<img width="634" height="333" alt="image" src="https://github.com/user-attachments/assets/2eb173cc-384a-4932-83ce-b33d87d373dc" />

  
### Linux File user categories:

In Linux, file and directory permissions control who can access and modify your data. These permissions are assigned based on three distinct categories of users:
* **Owner (`u`):** This is the specific user who owns the file or directory. Typically, it's the user who created it, but ownership can be changed. The owner has the most control and can set permissions for all three categories.
* **Group (`g`):** This refers to a designated group of users on the system. Any user who is a member of this group will have the permissions assigned to the group for that particular file or directory. This is useful for collaboration where multiple users need shared access.
* **Others (`o`):** This category includes all users on the system who are neither the file's owner nor a member of the file's assigned group. Permissions for "others" are often set to be more restrictive to maintain security.
