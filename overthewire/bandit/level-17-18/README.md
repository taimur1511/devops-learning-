# Bandit Level 17-18

## Challenge 

There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

## Solution 

I used the `diff` command followed by the files `passwords.new` and `passwords.old`. 

This then revealed two lines and since I inputted `passwords.new` first, the first output would be the password for the next level. 

<img width="1706" height="314" alt="image" src="https://github.com/user-attachments/assets/5702bf9d-de38-42d8-9658-7620848eb2d5" />

## What I learned

The `diff` command can be used to compare files and tell you what changes needed to be made to match them. 
