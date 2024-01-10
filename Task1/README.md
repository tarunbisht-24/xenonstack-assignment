Certainly! The internsctl command I've created supports various tasks based on the specified commands in Section A and Section B. Here's a summary of the tasks you can perform:

Make sure the script is executable by running:

--------------------
       chmod +x internsctl


Section A: Command Basics

1) Manual Page:

You can view the manual page by running:

--------------------
	man ./internsctl

This provides detailed documentation and usage guidelines for the internsctl command.

2) Help Option:

To view help and usage information, use:

--------------------
    /internsctl --help

3) Version Option:

To check the version of internsctl, use:
 
 --------------------
    ./internsctl --version

Section B: Task Execution

Part 1 | Level Easy

1) Get CPU Information:


--------------------
    ./internsctl cpu getinfo

This provides CPU information similar to the lscpu command.

2) Get Memory Information:

--------------------
    ./internsctl memory getinfo

This provides memory information similar to the free command.

Part 2 | Level Intermediate

3) Create a New User:

--------------------
    ./internsctl user create <username>

This creates a new user who can log in to the Linux system and access their home directory.

4) List All Regular Users:
  
--------------------
    ./internsctl user list

5) List Users with Sudo Permissions:

--------------------
    ./internsctl user list --sudo-only

Part 3 | Advanced Level

6) Get File Information:

--------------------
    ./internsctl file getinfo <file-name>
 
Provides detailed information about a file, including options for specific details.

Options:

6.1) To obtain the size of the specified file:
 
 -------------------- 
    ./internsctl file getinfo --size <file-name>

6.2) To obtain the permissions of the specified file:
 
-------------------- 
    ./internsctl file getinfo --permissions <file-name>

6.3) To obtain the owner of the specified file:
   
--------------------
    ./internsctl file getinfo --owner <file-name>

6.4) To obtain the last modified time of the specified file: 

--------------------
    ./internsctl file getinfo --last-modified <file-name>
