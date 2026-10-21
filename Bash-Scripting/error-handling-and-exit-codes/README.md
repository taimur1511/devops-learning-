# Error Handling & Exit Codes 

In Bash Scripting, error handling is detecting, managing and responding to errors when a script runs, rather than letting them go unnoticed. 

In the example below, I used arithmetic expansion to to divide the number 10 by the number 0. This shows an error in the output as 10 cannot be divided by 0 as this is a mathematical error. 

<img width="2712" height="386" alt="image" src="https://github.com/user-attachments/assets/e1d9b7be-25ac-4284-b620-5d377edf0235" />

To handle this error, I used an `if` statement which shows that if num2 is equal to 0, then output "Error: Division by zero is not allowed". This prints a clear error message to the terminal so the user understands why the calculation cannot continue. 

This is useful in error handling because it provides feedback instead of leaving the user wondering what went wrong.

I also used an exit code, `exit 1`, which terminates the script immediately and indicates that an error has occurred. Without this, the script could continue executing and potentially fail when it attempts to divide by zero.

<img width="2712" height="510" alt="image" src="https://github.com/user-attachments/assets/a60d20c3-c15c-486e-abf2-99c216f2c3e1" />

