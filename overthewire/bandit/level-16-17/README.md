# Bandit Level 16-17 

## Challenge 
The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. First find out which of these ports have a server listening on them. Then find out which of those speak SSL/TLS and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

## Solution 

I used `nmap -p 31000-32000 localhost` to scan the range 31000-32000. 

It returned five ports which had an open state. 

I then used `nmap -sV -p 31046,31518,31691,31790,31960 localhost` to scan the service and version for the five ports. 

Only ports 31518 a are using SSL.

<img width="1972" height="1428" alt="image" src="https://github.com/user-attachments/assets/7e72108c-e603-4e69-96bb-81a12b11f9d6" />

I used `openssl s_client -connect localhost: 31518` and `openssl s_client -connect localhost: 31790` and entered the password to the previous level and only the port 31790 returned Correct! whereas 31518 returned what I inputted. 

<img width="1454" height="1266" alt="image" src="https://github.com/user-attachments/assets/ffb2acb8-af11-484d-85c8-dca68d68c169" />

