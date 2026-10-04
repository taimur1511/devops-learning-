# Running scripts from anywhere 

In my previous notes I showed how `./` can be used to run a script in its current directory. 

What if we wanted to run the script anywhere without specifying its path? 

First we would need to place our script in a directory which is in the `PATH` environment variable. 

`PATH` is an environment variable which tells the Shell which directories to search for executable files in response to commands. 

From the below example, I added the file to a directory in the PATH environment variable. 

I added it to the `/usr/local/bin` using the `sudo` and `mv` command and made the file executable using `chmod +x`. 

So when I ran the file without specifying the directory, the Shell was able to find and execute the script. 


<img width="1756" height="216" alt="image" src="https://github.com/user-attachments/assets/a835b733-7c1e-4859-90c1-0a069bb8f723" />


