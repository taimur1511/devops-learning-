# Bandit Level 12-13

## Challenge 

The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Solution 

First I viewed the contents of data.txt using the `cat` command and it showed the below. 

<img width="1256" height="1404" alt="image" src="https://github.com/user-attachments/assets/30c11444-0c82-4c7c-8a4e-46e5e99fae27" />

I then created a working directory using `mktemp -d` 

I copied the file data.txt into the new directory using the `cp` command. 

I then navigated into the directory using `cd` and used `ls` to list the file. It showed data.txt which means the file was copied into the new directory. 

I then used `mv` to rename the file and used `ls` to check if the name had changed. 

<img width="1044" height="392" alt="image" src="https://github.com/user-attachments/assets/3d66b222-9940-4121-a69b-3b8b429968bf" />

This part took me a while as i had to continuously decompress files and used commands based off of the file type. The manual pages came in handy as they showed the commands i needed to use to decompress files. I also used available resources online.  

I had to keep decompressing and extracting files until it became an ASCII text file. 

<img width="1982" height="1390" alt="image" src="https://github.com/user-attachments/assets/5ea527f3-5fe3-44d4-b1de-a4aa0a97d66a" />

<img width="1982" height="580" alt="image" src="https://github.com/user-attachments/assets/6d1e9cf7-73ea-4cf0-9f0e-05a9fe878a3d" />

## What I learned

`xxd-r` converts the hexdump into its original binary file.

`gzip -d` can be used to decompress gzip files. 

`bzip2 -d` can be used to decompress bzip2 files. 

`tar xf` can be used to extract tar files. 



