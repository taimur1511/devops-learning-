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

## Set -e

`set -e` is a way of handling errors by telling the script to exit when a command fails. This is useful because it will prevent the script from carrying on when something has gone wrong. 

In the example below, the output shows "Before the script" and then an error. This is because we used `set -e` so the script will not carry on for a command which does not exist. In this case, "After the script" will not be displayed because the system does not recognise the command `nonexistentcommand`.     

<img width="2716" height="358" alt="image" src="https://github.com/user-attachments/assets/2104e497-646a-4beb-bd91-16446aac5fed" />

## Set -u 

`set -u` forces the script to stop if it encounters an unset variable. 

It helps prevent scenarios where missing data could lead to unexpected results. 

In the example below, the output shows an error. This is because I used `set -u` which forced the script to stop because `X` is an undefined variable. 

<img width="2732" height="238" alt="image" src="https://github.com/user-attachments/assets/4a388dc2-a7a7-47d5-b326-ee691fea0a3b" />

In another example, we see the same result because `W` is an undefined variable. 

<img width="2704" height="342" alt="image" src="https://github.com/user-attachments/assets/f92e6055-7567-43b9-bea8-4574b5f9003c" />

## set -x 
`set -x` prints each command that will be executed to the terminal before it is executed. This is helpful to follow the flow of a script. 

In the example below I used arithmetic expansion. In the terminal on the right, the commands have been printed. The value of Z is also printed. 

<img width="2712" height="428" alt="image" src="https://github.com/user-attachments/assets/7819cf2b-4fa7-464d-87d8-cf40f3cafe83" />

## Set -eux 
This allows you to combine all the `set` commands listed above and use them together. This will stop the script if there is error because of `e`, an unset variable because of `u` and will print the commands in the terminal because of `x`. 

In the below example, the terminal prints each command before executing. It does not proceed with an unset variable and stops at a command that doesn't exist. 

<img width="2670" height="416" alt="image" src="https://github.com/user-attachments/assets/ebbe1d62-8737-439c-baf7-efca7e247670" />

## More Set Commands 
- `set -o nounset` which can be used in the same way as `set -u`. 
- `set -o errexit` which can be used in the same way as `set -e`.
- `set -o pipefail` helps detect when a command fails inside a pipeline. In the example below, the `cat` command fails because of the file not existing, therefore causing the whole pipeline to fail so the `grep` command will not even run.

<img width="2716" height="350" alt="image" src="https://github.com/user-attachments/assets/41188780-5de4-4cdb-a9fa-ad643534e337" />







