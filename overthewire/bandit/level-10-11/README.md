# Bandit Level 10-11 

## Challenge 

The password for the next level is stored in the file data.txt, which contains base64 encoded data

## Solution 

<img width="1314" height="338" alt="image" src="https://github.com/user-attachments/assets/86745d94-c28d-46d8-bb4b-fcd7a6c47b45" />

First I used `cat` to view the contents of the files data.txt 

The output displayed a line of random upper case and lower case letters followed by ==. 

From the challenge description i can see that this file contains base64 encoded data. 

I used `man base64` to show me the manual page for base 64. 

After reading through it I learned that `base64 -d` can be used to decode data. 

## What I Learned

`base64` can be used to encode and decode data and print to a standard output. 

`-d` can be used to decode data. 




