# Level 13-14 

## Challenge 

The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Look at the commands that logged you into previous bandit levels, and find out how to use the key for this level.
If you need help with this level: a hint file can be found in the home directory.
Make sure to read the error messages as they are informative.

## Solution 

I first logged into the server as bandit13 and found the file `sshkey.private`.

I used `scp` to securely copy the `sshkey.private` file from the Bandit server to my local Ubuntu machine. 

The `-P 2220` option specifies the SSH port used by the Bandit server. `bandit13@bandit.labs.overthewire.org` identifies the remote user and server, while /home/bandit13/sshkey.private specifies the file I wanted to copy. The `.` at the end means the file was copied into my current directory.

<img width="1972" height="728" alt="image" src="https://github.com/user-attachments/assets/83dff64f-af9f-44df-8b82-9d70200ddb6b" />

Now that the file was copied to my local Ubuntu machine i viewed the permissions of the file and saw that they were `-rw-r-----`. This shows the owner does not have execute permissions. 

I then used a chmod calculator to find the correct numerical permissions to allow the owner to execute. 

I then used the argument `-i` after ssh to use the private key to authenticate me. I then followed it with `bandit14@bandit.labs.overthewire.org -p 2220`. 

<img width="1910" height="406" alt="image" src="https://github.com/user-attachments/assets/59a75209-91e5-4ac2-b7fe-4281a10359e7" />

I then used the `cat` command to view the contents of the file and get the password. 

<img width="1630" height="128" alt="image" src="https://github.com/user-attachments/assets/97f0ac6c-b3a2-4613-a30f-a953d61daf44" />

## What I learned. 

How to use `scp` to securely copy a file from a remote server to my Ubuntu machine. 

How to use an SSH private key for authentication instead of a password.

How the `-i` argument specifies the private key to use. 




