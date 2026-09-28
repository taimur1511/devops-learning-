# Bandit Level 18-19 

## Challenge 

The password for the next level is stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

## Solution 

For this, I logged into bandit18 as normal using SSH but at the end i added the condition `cat readme`. Therefore the command was executed from my machine rather than from inside the bandit server. 

<img width="1246" height="502" alt="image" src="https://github.com/user-attachments/assets/3a7e0df1-0da7-48d6-9967-d7406cb3d54a" />





