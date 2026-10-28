# Challenge 3: File Checker with Permissions

Create a script that checks if a file exists and displays its permissions.

Requirements:
- Prompt user for a filename
- Check if the file exists
- If it exists, check if it's readable, writable, and executable
- Display appropriate messages for each permission

For this exercise, I used nested `if` statements to check whether a file exists and what the permissions are. 

I first used the `read` command to accept a filename from the user and store it in a variable called `file1`

I then created an `if` statement using `-f` to check whether the path exists and points to a regular file. 

If the file exists, the script runs three separate `if` statements to check whether the file is readable `-r`, writable `-w` and executable `-x`.

Depending on whether each condition is true or false, the script displays an appropriate message in the terminal. If the file does not exist, it displays an error message instead.

<img width="2766" height="1238" alt="image" src="https://github.com/user-attachments/assets/abc282ec-4b33-4471-b795-d742ed26a989" />

