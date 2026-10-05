# Variable and Parameters

## Variables 

Variables allow you to store and manipulate data. Variables are used to store values that can be accessed and modified throughout the script.  

In the below example, I have created different variables. `greeting`, `count`, `fruits` and `name`. 

<img width="1876" height="490" alt="image" src="https://github.com/user-attachments/assets/7db0f4c5-e260-4498-8530-48cf1886de0b" />

The `$` means "get the value stored in this variable" 

For `echo "Hello" $name`, this displays the word `Hello` followed by the value stored in the `name` variable.

For example, if `name="Taimur"`, the output will be:

```
Hello Taimur
```

`$name` tells Bash to use the value stored in the `name` variable.



This is what the output looks like in the terminal. 

<img width="1776" height="272" alt="image" src="https://github.com/user-attachments/assets/fe505546-39f7-44dd-a33a-59821c1cbb12" />

## Parameters 

Parameters are values that you give to a script when you run it. They allow the script to use different information without changing the script itself.

In this example I used three Parameters. 

`$1`, `$2`, and `$3` represent the first, second, and third parameters passed to the script.

I also used `$@` to display all of the parameters that were passed to the script.

<img width="1932" height="358" alt="image" src="https://github.com/user-attachments/assets/a5145b54-7013-4e38-bc76-ca246be71942" />

This is how it was displayed when I ran the script in my terminal. 

`hello`, `hi` and `hey` are arguments passed to the script. Depending on the order, they will correspond with the first, second or third Parameter. 

<img width="1840" height="338" alt="image" src="https://github.com/user-attachments/assets/a0bba29c-b282-474d-8df4-ea330f7b3614" />

## Arithmetic Expansion 

Arithmetic Expansion in Bash allows you to perform maths calculations in a script. 

In the below example, I created two variables, `num1` and `num2` and assigned them values `3` and `15`. 

I then used arithmetic expansion `$(( ))` to add the two values together and store the result in a variable called `result`.  

I then used `echo` to display the calculations in my terminal. 

<img width="1754" height="352" alt="image" src="https://github.com/user-attachments/assets/9f119081-7534-431a-9b7a-f715d0ab3669" />

<img width="1770" height="86" alt="image" src="https://github.com/user-attachments/assets/f2f26628-e5d9-4b5c-8ea5-3a086d0d49f5" />








