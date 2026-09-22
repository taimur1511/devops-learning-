# Bandit Level 4-5 

## Challenge 

The password for the next level is stored in the only human-readable file in the inhere directory.

## Solution 

<img width="1512" height="1038" alt="image" src="https://github.com/user-attachments/assets/3518e0be-3719-4cc8-8e3f-35026d8e2ecf" />

I used `ls` to list files and directories.  

I used `cd` to navigate into the inhere directory. 

`ls` to list files and directories for inhere. 

`ls -l` to list files in a more detailed format.

`file ./*` is used to tell me what type everything is in this directory. 

It showed me that ./-file07 is ASCII text which is standard readable text. 

I then used cat ./-file07 to display the contents of that file in the current directory. 

## What i Learned 

How to use `file` to identify the type of file such ASCII text. 

How to use `./*` as a wildcard to target files within the current directory. 








