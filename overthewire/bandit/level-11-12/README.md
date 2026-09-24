# Level 11-12

## Challenge 

The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Solution 

<img width="1128" height="378" alt="image" src="https://github.com/user-attachments/assets/fae99374-3a45-4b0c-bcc1-68051c0847ac" />

Before I started to find the password, on this level there was some helpful reading material called Rot13. Rot13 is a simple substitution where each letter is shifted 13 places through the alphabet. For example, if i was to run Rot13 on the word 'linux' the output would be 'yvahk'. 

I first used `cat file.txt` followed by the the `|` command. This is so the terminal takes the output from `cat` and sends it into the next command. 

After `|` I used `tr 'A-Za-z' 'N-ZA-Mn-za-m'`. The `tr` command which takes characters from one set and replaces them with characters from another set. 

For what followed after `tr` I had to do my own research and figure what I needed to use in order to shift all lowercase and uppercase letters by 13 positions. 

`A-Za-z` represents all uppercase and lower case letters. 

`N-ZA-Mn-za-m` is a sequence which will replace the letters above. The N will replace the A as it is 13 positions from A. The M will replace the Z as it is also 13 positions from Z and so on. 

## What I Learned 

Rot13 can be used to to shift letters 13 places in the alphabet. 

`tr` command can be used to replace characters from one set with another. 




