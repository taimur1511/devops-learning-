# Functions And Inputs 

Functions and inputs help you organise your code and allow your scripts to work with different information.

## Functions 

In the example below, I created a function called `hello_world`. I then used `echo` to display "Hello World!". 

I then created another function called `greet_person` and used `local` to create a variable `name` assigning it the first argument passed to the function. 

I then used `echo` to output "Hello", followed by the value stored in the `name` variable. 

`greet_person "Taimur"` will then display Hello, Taimur! 


<img width="2686" height="506" alt="image" src="https://github.com/user-attachments/assets/756e57b4-2e4e-4b02-8e6c-1ce0b71570ec" />

## Parameters 
Parameters allow us to pass data to functions to perform specific tasks based on provided inputs. 

In the example below. I created a function called `print_names`. 

I used the special parameter `$#` which holds the count of arguments. 

I also used the special parameter `$0` which contains the name of the script. 

The special parameter `$@` is used to display all arguments when the script is called. 

I then used `print_names` to call the script. 

<img width="2748" height="564" alt="image" src="https://github.com/user-attachments/assets/ff96fa10-6724-4d1d-ab2a-23725f0cce18" />

As you can see, the output shows the number of names, the script name, the first and second name and all the names. 

## User Inputs
User inputs allows the script to interact with users and make them more dynamic and responsive. 

In the example below, I created a function called `greet_user`. I used the `read` command to capture the user input and store it in the variable `name`. 

On the Terminal on the right, I ran the command and it displayed "What is your name?". I then inputed my name which then displayed "Hello, Taimur!" 

<img width="2654" height="480" alt="image" src="https://github.com/user-attachments/assets/269f36be-d55d-46bb-8841-9ac6810321bc" />



