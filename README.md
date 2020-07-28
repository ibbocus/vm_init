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



| Command                                     | Explanation                                                                                                                                                                                                                                                    |
| ------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `chmod a+r _publicComments.txt_`            | adds read permission for all classes (i.e. _**u**ser_, _Group_ and _Others_)                                                                                                                                                                                   |
| `chmod a-x _publicComments.txt_`            | removes execute permission for all classes                                                                                                                                                                                                                     |
| `chmod a+rx _viewer.sh_`                    | adds read and execute permissions for all classes                                                                                                                                                                                                              |
| `chmod u=rw,g=r,o= _internalPlan.txt_`      | sets read and write permission for _**u**ser_, sets read for _Group_, and denies access for _Others_                                                                                                                                                           |
| `chmod -R u+w,go-w _docs_`                  | adds write permission to the directory _docs_ and all its contents (i.e. **R**ecursively) for owner, and removes write permission for group and others                                                                                                         |
| `chmod ug=rw _groupAgreements.txt_`         | sets read and write permissions for _**u**ser_ and _Group_                                                                                                                                                                                                     |
| `chmod 664 _global.txt_`                    | sets read and write permissions for _**u**ser_ and _Group_, and provides read to _Others_.                                                                                                                                                                     |
| `chmod 744 _myCV.txt_`                      | sets read, write, and execute permissions for _**u**ser_, and sets read permission for _Group_ and _Others_                                                                                                                                                    |
| `chmod 1755 _findReslts.sh_`                | sets sticky bit, sets read, write, and execute permissions for owner, and sets read and execute permissions for group and others (this suggests that the script be retained in memory)                                                                         |
| `chmod 4755 _setCtrls.sh_`                  | sets _[UID](https://en.wikipedia.org/wiki/Setuid "Setuid")_, sets read, write, and execute permissions for _**u**ser_, and sets read and execute permissions for _Group_ and _Others_                                                                          |
| `chmod 2755 _setCtrls.sh_`                  | sets _[GID](https://en.wikipedia.org/wiki/Setgid "Setgid")_, sets read, write, and execute permissions for _**u**ser_, and sets read and execute permissions for _Group_ and _Others_                                                                          |
| `chmod -R u+rwX,g-rwx,o-rx _personalStuff_` | **R**ecursively (i.e. on all files and directories in _personalStuff_) adds read, write, and special execution permissions for _**u**ser_, removes read, write, and execution permissions for _Group_, and removes read and execution permissions for _Others_ |
| `chmod -R a-x+X _publicDocs_`               | **R**ecursively (i.e. on all files and directories in _publicDocs_) removes execute permission for all classes and adds special execution permission for all classes                                                                                           |





