# Bandit Level 12-13

## Challenge 

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Solution 

<img width="1256" height="1404" alt="image" src="https://github.com/user-attachments/assets/30c11444-0c82-4c7c-8a4e-46e5e99fae27" />

First I viewed the contents of data.txt using the `cat` command and it showed the above. 

<img width="1044" height="392" alt="image" src="https://github.com/user-attachments/assets/3d66b222-9940-4121-a69b-3b8b429968bf" />

I then created a working directory using `mktemp -d` 

I copied the file data.txt into the new directory using the `cp` command. 

I then navigated into the directory using `cd` and used `ls` to list the file. It showed data.txt which means the file was copied into the new directory. 

I then used `mv` to rename the file and used `ls` to check if the name had changed. 

<img width="1044" height="392" alt="image" src="https://github.com/user-attachments/assets/30eb6625-3101-49e6-9cad-89b9a45ef6b0" />

