# Conditionals 

## if Statements 

If statements allow you to introduce decision making logic to your script. 

If statements start with `if` and end with `fi`. 

Some examples of If statements. 
<img width="1434" height="396" alt="image" src="https://github.com/user-attachments/assets/5b4f7ef6-f4f1-422d-bb42-6a4b68088990" />

In this example, I created a variable (grade) and assigned it a number (92). 

I then used `if [ $grade -ge 90 ] && [ $grade -le 100 ]`. 

What this means is that If the grade is greater than 90 & less than 100 then the output should display "Excellent! You got an A." 
<img width="2756" height="422" alt="image" src="https://github.com/user-attachments/assets/25066120-0925-4e92-bc2f-48d624b79225" />

Another example. 
<img width="2764" height="372" alt="image" src="https://github.com/user-attachments/assets/d8013cdf-3972-4b18-baa3-8fa45fe84997" />

## else and elif
`else` runs when none of the previous conditions are true. 

`elif` means "else if". This allows you to check another condition if the previous `if` condition was false. 

In this example I created the variable Temperature and assigned it a value of 25. 

The code below means, if the Temperature is greater than 15, then display "It is Hot outside.". Otherwise if the Temperature is equal to 15 then display "It is Warm outside." If it is neither greater than 15 or equal to 15 then display "It is Cold outside." 

<img width="2752" height="558" alt="image" src="https://github.com/user-attachments/assets/7face270-db8e-4eec-9725-f0343d6f6c27" />

## Nested if Statements 

Nested if statements allow us to create more complex decision making structures by embedding if statements within other if statements. 


In this example, I created variables `age` and `grade` and assigned them each a numerical of 18 and 85. 

The code below shows, that if the age is greater than or equal to 18 and the grade is greater than or equal to 80 then the following output will be shown, 

"You are eligible based on age.

You are eligible based on grade.

Congratulations! You are eligible for a Scholarship!" 


If we were to keep the age the same and change the grade to 75, as the grade is below 80, the output would show "You are eligible based on age.

Sorry, your grade is not high enough." 


However, if we were to reduce the age down from 18 and reduce the grade down from 80, then the output will show "Sorry, you are not eligible. " 

<img width="2664" height="688" alt="image" src="https://github.com/user-attachments/assets/012d9a95-3554-4001-9967-2884fe7da4ea" />
