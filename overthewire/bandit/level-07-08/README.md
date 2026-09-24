# Bandit Level 7-8

## Challenge 

The password for the next level is stored in the file data.txt next to the word millionth. 

## Solution 

First I used `cat data.txt` to view the contents of the file data.txt. 

This returned a long list of words followed by a combination of random letters. 

I knew I had to narrow my search so i used the `grep` command followed by the word millionth. This then returned the line containing the word millionth allowing me to identify the password next to it. 

<img width="1024" height="178" alt="image" src="https://github.com/user-attachments/assets/c149259c-d345-4dfc-8304-72def14a9f39" />

## What I Learned 

The `grep` command can be used to search for specific strings within text, in this instance the word millionth.
