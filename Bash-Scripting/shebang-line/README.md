# The 'Shebang' Line

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
