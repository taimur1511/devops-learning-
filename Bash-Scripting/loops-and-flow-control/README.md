# Loops and Flow Controls 

Loops allow you to repeat a set of commands multiple times. Flow control determines how a script runs, including when to repeat commands, make decisions, or stop.

## while Loops 

`while` loops allow you to repeatedly execute a block of code as long as a certain conditions stays true. They allow you to execute a block of code until a specific condition becomes false. 

For `while` loop statement the code is written between `do` and `done`. 

In this example, I created a variable called count and assigned it the value 1. 

I then used `while` to repeat a set of commands as long as count was less than or equal to 5. 

Inside the loop I used `echo` to display the current value of count followed by `((count++))` which increased the value by 1 each time the loop runs. 

The output shows that the loop repeats until the count reaches 5. After displaying 5, the count increases to 6, making the condition false and causing the loop to stop.


<img width="2566" height="374" alt="image" src="https://github.com/user-attachments/assets/4112d262-959a-4c71-a150-73e5fd454009" />

In the below example I created an array containing three items. 

I then created a variable called `index` and assigned it the value 0. This is used to track the current position in the array. 

The `while` loops repeats as long as `index` is less than the number of items in the array. 

`echo` displays the fruit at the current index, and `((index++))` increases the index by 1 each time the loop runs.

Once the index reaches the number of items in the array, the condition becomes false and the loop stops.

<img width="2572" height="360" alt="image" src="https://github.com/user-attachments/assets/926771c7-9692-45ee-b161-12d6d0297142" />

## for Loops 

`for` loops enable you to repeat a block of code for a specified number if iterations. 

For `for` loops the code is written between `do` and `done`. 

In the below example, I created a for loop that uses the `seq` command to generate numbers from 1 to 7 and stores each number in the variable `number` as the loop runs.


<img width="2716" height="428" alt="image" src="https://github.com/user-attachments/assets/5b87382e-56cf-422b-bd98-7f473b774cde" />

## break and continue 

These statements provide additional control within `for` and `while` loops. They allow you to interrupt or skip iterations based on specific conditions. 

The `break` statement immediately exits the inner most loop it is placed in regardless of the loops condition. 


In the example below, I created a `for` loop. I created the variable `i` and assigned it the number 1. I then followed this up with `i<=5` which means the loop continues as long as `i` is less than or equal to 5. `i++` increases the variables value by 1 each time the loops runs. 

`if [ $i -eq 3 ]` checks if the variables value is equal to 3. If the condition is true, the `break` statement stops the loop immediately. 

The output displays `Number:1` and `Number:2` but does not run Number:3 or anything after up until 5 because of the `break` statement. 

<img width="2650" height="402" alt="image" src="https://github.com/user-attachments/assets/0b278890-9185-46a6-b522-2f23969f699e" />

The `continue` statement allows you to skip the current iteration and move on to the next iteration of the loop. 

In the example below, I replaced the `break` statement with the `continue` statement. 

The `continue` statement will skip the iteration if the variables value is equal to 3. 

The output therefore displays 

`Number: 1`

`Number: 2`

`Number: 4`

`Number: 5`

and skips `Number:3`. 


<img width="2652" height="386" alt="image" src="https://github.com/user-attachments/assets/cb56d03f-efeb-4c68-a00d-b3822bbd1ecc" />






