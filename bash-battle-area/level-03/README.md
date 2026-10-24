# Level 3: Conditional Statements

Mission: Write a script that checks if a file named hero.txt exists in the Arena directory. If it does, print Hero found!; otherwise, print Hero missing!.

## Solution 

I created a variable called `file` and assigned `./arena/hero.txt` to it. `./arena` is the directory and `hero.txt` is the file i'm checking. 

I then used `if [ -f $file ]`.  

- `if` is telling the script to make a decision based off of the condition.
- `-f $file` checks whether the file exists in the specified location. 
- `echo` displays a message in the terminal.
- If the condition is true, the script outputs Hero found!.
- If the condition is false, the `else` block runs and outputs Hero missing!.

As there is no file called `hero.txt` under the directory `arena`, the script outputs Hero missing! 

<img width="2732" height="606" alt="image" src="https://github.com/user-attachments/assets/8f09ebfc-7ea4-42e3-936d-91cf168bdea1" />
