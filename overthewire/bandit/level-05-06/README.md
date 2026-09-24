# Bandit Level 5-6 

## Challenge 

The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable

1033 bytes in size

not executable

## Solution 

<img width="1582" height="1070" alt="image" src="https://github.com/user-attachments/assets/dc468752-a8d5-49d9-8bcd-fecd14e9dc72" />

I first used `ls` to list the files and directories and navigated into the inhere directory using `cd`. 

Used `ls` and `ls -l` to list the files and directories. 

I then navigated into a random directory, in this instance maybehere02 and then viewed the content of -file3 within that directory. 

The following is what it showed me. 

<img width="1982" height="1406" alt="image" src="https://github.com/user-attachments/assets/1ae4d2c8-7354-4569-ad8c-8b388668d1c1" />


It would take me a lot of time to search through each directory and each file within those directories manually so I used the following: 

<img width="1318" height="210" alt="image" src="https://github.com/user-attachments/assets/f8e5cb7b-8331-4370-abd2-9a1730703158" />

I used `find -type f` to search for regular files within the inhere directory and its subdirectories.

I then added `-size 1033c`, which searches for files that are exactly 1033 bytes in size.

This returned ./maybehere07/.file2, which matched the file size requirement.

I then used `cat ./maybehere07/.file2` to display the contents of the file.

## What I Learned 

How to use `find -type f` to search specifically for regular files.

How to use `-size 1033c` to search for a file which is exactly 1033 bytes in size. 

How the c in `-size 1033c` stands for bytes.

How to use a file path such as `./maybehere07/.file2` to access a specific file within a subdirectory. 

I learned that the file path can change depending on my current working directory. For example, if I was in the home directory, I could use cat ./inhere/maybehere07/.file2 to access the same file. 




