# Bandit Level 19-20 

## Challenge 

To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

## Solution 

First I used `ls -l` to view the owner and permissions of the setuid binary. 

It shows that the owner is bandit20 and the group is bandit19 and the permissions `-rwsr-x---` show that the user bandit19 can execute the binary but it is executed as bandit20. 

I then used `./bandit20-do cat /etc/bandit_pass/bandit20` to run bandit20-do from the current directory and to view the contents of the location of the password. 

<img width="1642" height="366" alt="image" src="https://github.com/user-attachments/assets/758c0893-c662-4b7f-af66-a8df09eec8c7" />

## What i Learned 

`./` is used to run a programme from the current directory 

`s` (SUID) in this chase `-rwsr-x---` allows a program to run with the permissions of its owner (bandit20). 

SUID can be used to allow a program to perform actions with another users permissions.



