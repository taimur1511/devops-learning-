# Bandit Level 15-16 

## Challenge 

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.

## Solution 

For this level I had to do some research into SSL/TLS. 

I used the command `openssl s_client -connect localhost:30001` 

`openssl` opens the OpenSSL toolki.

`s_client` starts OpenSSL's SSL/TLS client.

`-connect` specifies the server and port to connect to.

`localhost:30001` connects to port 30001 on my Ubuntu machine.

I then entered the password for the previous level and it read Correct! and gave me the password for the next level. 

<img width="1930" height="1304" alt="image" src="https://github.com/user-attachments/assets/52787bba-d9d7-431d-b8c3-4a6dd70d57d1" />

## What I learned 

`nc` is not suitable for every network connection because some services require SSL/TLS encryption. 

`openssl s_client` can be used to establish an SSL/TLS connection to a specific host and port.

`-connect` is used to specify the destination such as localhost:30001. 
