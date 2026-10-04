# Intro  


## The 'Shebang' Line

A Shebang Line tells the operating system which interpreter should be used to run a script. 

For example: `#!/bin/bash`. 

`#!` identifies the line as a shebang

`/bin/bash` tells the system to use bash to interpret the script. 


## Practical Example

In the below I used the `touch` command to create a file called `example.sh`. 

I then used `vim` to open up a text editor in my terminal to write a bash script which can be seen in the second screenshot. 

I had to use `chmod +x` to give it executable permissions. 

There were three ways I executed the script. 

First I used `./` to run `example.sh`. This tells the shell to run the script from the current directory. 

I also used `sh` and `bash`. These commands specify which interpreter should be used to run the script.

<img width="1630" height="528" alt="image" src="https://github.com/user-attachments/assets/4c4ca481-aae9-4d78-abd3-62dcf3257fb0" />

Below is the bash script I wrote which can be executed using `./`, `sh` and `bash`. 

<img width="1994" height="528" alt="image" src="https://github.com/user-attachments/assets/7a44b4dc-e1c8-4929-b288-c3d5d5c4e2cf" />


## Comments 

Comments are lines in a script that are not executed as part of the code. They serve as informative text for the reader. 

There are two types of comments. Single line comments and multiline comments. 

`#` is used to make a single line comment. 

`:` followed by `''` is for a multiline comment. The multiline comment will be whatever is inputed in the single quotation marks. See example below. 

<img width="1488" height="564" alt="image" src="https://github.com/user-attachments/assets/75eabe9b-0a02-4e2e-813f-cf364f821dee" />

As you can see below, if you were to run the file `example.sh` using `./` it will not show the comments. 

<img width="1394" height="238" alt="image" src="https://github.com/user-attachments/assets/45d9903c-9b30-40a4-9e49-6f13e440f1a0" />

Comments can be read in the terminal by using the `cat` command followed by the filename. 


## Running scripts from anywhere 

In my previous notes I showed how `./` can be used to run a script in its current directory. 

What if we wanted to run the script anywhere without specifying its path? 

First we would need to place our script in a directory which is in the `PATH` environment variable. 

`PATH` is an environment variable which tells the Shell which directories to search for executable files in response to commands. 

From the below example, I added the file to a directory in the PATH environment variable. 

I added it to the `/usr/local/bin` using the `sudo` and `mv` command and made the file executable using `chmod +x`. 

So when I ran the file without specifying the directory, the Shell was able to find and execute the script. 


<img width="1756" height="216" alt="image" src="https://github.com/user-attachments/assets/a835b733-7c1e-4859-90c1-0a069bb8f723" />



