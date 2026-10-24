# Level 2: Variables and Loops

Mission: Create a script that outputs the numbers 1 to 10, one number per line.

## Solution 

For this level, I created a variable called `number` and stored the value 1 in it. I then used the `while` loop to repeatedly execute a block of code as long as the condition stays true. 

In this case the condition is `[ $number -le 10 ]`. 

- `$number` is a variable expansion. The `$` tells the script to retrieve the value stored in the variable `number`.
- `-le 10` tells the script to retrieve values as long as they are less than or equal to 10.
- `((number++))` is an arithmetic operation which tells the script to increase the value of the variable `number` by 1.

In brief, this block of code is telling the script to increase the value of the variable `number` by 1 as long as `$number` is less than or equal to 10. The script stops once the condition is no longer true. 

<img width="2714" height="616" alt="image" src="https://github.com/user-attachments/assets/79b2ac8a-28e6-47c4-8581-58b300e47cef" />

