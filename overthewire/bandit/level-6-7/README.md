# Challenge 

The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7

owned by group bandit6

33 bytes in size

## Solution 

<img width="1786" height="1384" alt="image" src="https://github.com/user-attachments/assets/ac8f5d52-a394-443e-982b-cf339f559175" />

Initially I tried searching the server using `find /` followed by the user, group and file size conditions. 

This returned the matching file but also produced a long list of permission denied messages because i didn't have permissions to access certail directories. 

<img width="1258" height="194" alt="image" src="https://github.com/user-attachments/assets/af4d67e0-da6b-4b6b-99a2-8daa5c811973" />

I then used the same command as above but added `2>/dev/null`. This hides the permission error messages making the output easier to read and allowing me to find files that match my search criteria. 

I then used the `cat` command to view the contents of the file. 

## What I Learned 

`find /` searches from the root of the filesystem allowing me to search across the server. 

Conditions can be combined with `file /` to search for specific files based on properties e.g. owner, group and file size. 

`2>/dev/null` hides error messages such as permission denied making the output easier to read. 




