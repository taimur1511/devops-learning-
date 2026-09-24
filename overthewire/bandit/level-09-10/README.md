# Bandit Level 9-10 

## Challenge

The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## Solution 

<img width="1254" height="250" alt="image" src="https://github.com/user-attachments/assets/a46209e1-11c2-4607-8568-e7d5ee12175d" />

I used the `strings` command to view printable strings in data.txt. 

I also used `|` to combine the previous command with the following one. 

I finally used the `grep` command to search for anything containing ===.

## What I Learned 

`strings` can be used to find printable strings within a file. 

