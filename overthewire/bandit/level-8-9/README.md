# Bandit Level 8-9 

## Challenge 

The password for the next level is stored in the file data.txt and is the only line of text that occurs only once. 

## Solution 

First I used `cat data.txt` to view the contents of the file. 

Once again it returned a long list. 

<img width="948" height="220" alt="image" src="https://github.com/user-attachments/assets/8173aaee-1679-4787-a4b8-9faf0adfc2c2" />

I then used `sort` which takes all the lines in data.txt and puts them in alphabetical and numerical order. 

I then used `|` to take the output from `sort` and send it to the next command. 

I then used `uniq -u`. `uniq` looks at identical lines next to each other and removes repeated lines. `-u` only shows me lines that are unique. 

## WHat I Learned 

`sort` can be used to put lines in a file in alphabetical and numerical order 
`uniq` can be used to look at identical lines next to each other and remove repeated lines. 

