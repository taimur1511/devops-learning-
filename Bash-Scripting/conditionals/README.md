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

