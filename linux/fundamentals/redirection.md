# Linux Redirection

Linux redirection allows the input and output of commands to be redirected to or from files instead of only being displayed in the terminal.

## Output Redirection

The `>` operator can be used to redirect the output of a command into a file.

For example:

echo "Hello Linux" > example.txt

This creates example.txt and writes Hello Linux into the file.

If the file already contains information, using > will overwrite the existing content.

The `>>` operator can be used to append output to a file instead.

echo "Another line" >> example.txt

This adds the new text to the end of the file without removing the existing content.

## Input Redirection

The `<` operator can be used to provide input to a command from a file.

For example:

cat < example.txt

This takes the contents of example.txt as input for the cat command.

## Practical Example

<img width="459" height="211" alt="image" src="https://github.com/user-attachments/assets/0b972835-e029-4044-adb6-fd03b8801766" />


- I first used `>` to redirect the output of echo into a file: echo "Hello World" > redirection.file
- I then used `cat` to view the contents of the file. The output was: Hello World
- I then used `>>` to append additional text to the file: echo "Hello World2" >> redirection.file
- I used `cat` again to view the contents: Hello World, Hello World2
- Finally, I used `<` to redirect the contents of the file as input to the cat command: cat < redirection.file. 
