### Manipulating files/directories
- learning to move files from local machine to the virtual machine 
- to do so we use the sink_files feature in vagrant

### Error handling 
- running the vm this morning returned the error that "the vm was creatred with a user that doesnt match the current user 
- check hidden files - using the command ls -a 
- remove .vagrant file

## Communications with developers - to understand requirements 
- what language is used to build the app
- what framework has been used - mvc, react(front-end) 
- what are the dependencies and which ones have been included and which ones are needed 
- what will the app look like 

## install dependencies on ruby 
- install bundler in root mode using sudo -i 
- exit sudo and run the command bundle to download and install dependencies 

## run the test rake test 
- gives you the instructions to pass all the test

enter the vm 
- sudo apt-get updates
- sudo apt-get install "package"
- sudo apt-get upgrade 
- systemctl status nginx (name of the program)

- go back to vm install node.js

- use curl to install packages that or not in a package directory 

- in order to install pm2 
- install nom first in sudo 

- npm package manager for node

### bash scripting 

- bash scripts can help us automate processes
.sh means it is an executable file 

chmod - change mode on linux bash - make files executable +x name_of_file
- syntax to make a file executable +x 
- to run the executable file:
./name_of_file 

## created an bash script which downloaded nginx again onto our device 
-#!/bin/bash
- sudo apt-get update
- sudo apt-get install nginx 
- sudo apt-get upgrade

credit @ Bari


## Bash Commands

top - shows a list of all the processes currently running
ps - shows the program id's
chmod +x <filename.sh> - Changes the mode of a file to make it executable




| Number | Octal Permission Representation                           | Ref  |
| ------ | --------------------------------------------------------- | ---- |
| **0**  | No permission                                             | \--- |
| **1**  | Execute permission                                        | \--x |
| **2**  | Write permission                                          | \-w- |
| **3**  | Execute and write permission: 1 (execute) + 2 (write) = 3 | \-wx |
| **4**  | Read permission                                           | r--  |
| **5**  | Read and execute permission: 4 (read) + 1 (execute) = 5   | r-x  |
| **6**  | Read and write permission: 4 (read) + 2 (write) = 6       | rw-  |
| **7**  | All permissions: 4 (read) + 2 (write) + 1 (execute) = 7   | rwx  |









