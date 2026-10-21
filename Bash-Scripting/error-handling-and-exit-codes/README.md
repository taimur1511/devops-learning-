# Error Handling & Exit Codes 

## Error Handling

In Bash Scripting, error handling is detecting, managing and responding to errors when a script runs, rather than letting them go unnoticed. 

In the example below, I used arithmetic expansion to to divide the number 10 by the number 0. This shows an error in the output as 10 cannot be divided by 0 as this is a mathematical error. 

<img width="2712" height="386" alt="image" src="https://github.com/user-attachments/assets/e1d9b7be-25ac-4284-b620-5d377edf0235" />

To handle this error, I used an `if` statement which shows that if num2 is equal to 0, then output "Error: Division by zero is not allowed". This prints a clear error message to the terminal so the user understands why the calculation cannot continue. 

This is useful in error handling because it provides feedback instead of leaving the user wondering what went wrong.

I also used an exit code, `exit 1`, which terminates the script immediately and indicates that an error has occurred. Without this, the script could continue executing and potentially fail when it attempts to divide by zero.

<img width="2712" height="510" alt="image" src="https://github.com/user-attachments/assets/a60d20c3-c15c-486e-abf2-99c216f2c3e1" />

## Exit Codes 
Exit codes are a numerical value which are returned to the system when a command or script ends. 

An exit code of `0` represents success. Any non 0 exit code represents an error. 

In the example below, I used the command `command -v` to check whether the `git` command is available on the system. `2>/dev/null` redirects error messages to /dev/null, preventing them from being displayed in the terminal.

`$?` is the exit status of the the last executed command. 

`if [[ $? -ne 0 ]]` shows, that if the exit status of the last executed command is not equal to 0 then the terminal will output, "git is not installed. Please install git.". This is followed by `exit 1` to immediately terimante the script. 

I then used the `else` statement to display "git is installed" if `if [[ $? -ne 0 ]]` was not true. 


<img width="2758" height="428" alt="image" src="https://github.com/user-attachments/assets/087aaa19-4cf0-4381-a350-925d838faf96" />
