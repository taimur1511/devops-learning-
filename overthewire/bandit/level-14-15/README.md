# Bandit Level 14-15

## Challenge 

The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

## Solution 

I used `nmap -p 30000 -sV localhost` to scan port 30000 on the local Bandit server. 

`-p 30000` specifies the port I wanted to scan, while `-sV` attempts to identify the service and version running on that port. 

`localhost` refers to the machine I am currently connected to.

This returns the below. 

<img width="1998" height="894" alt="image" src="https://github.com/user-attachments/assets/b7935f1d-f96a-40a2-8de0-16f659fc170f" />

I used `nc localhost 30000` to connect to the service running on port 30000 on the local Bandit server. 

I then entered the password from the previous level. 

The service returned Correct! and provided the password for the next level.

<img width="1896" height="160" alt="image" src="https://github.com/user-attachments/assets/1db098df-f9e5-4cc6-af1d-0d19dc539319" />

## What I learned 

`nmap` can be used to scan ports and identify services running on a server.

`-sV` identifies the service and version running on the port.

`localhost` refers to the machine I am currently connected to.

`nc` (Netcat) can be used to connect to a specific port.

