# Environment Variables 

Environment variables allow us to store and retrieve important information within the Bash script.  They are like a container which store valuable information for the script. They provide a way to store settings and config that the script can access when needed. 

## Reading Environment Variables 

In the example below, the script shows how to read and display environment variables in Bash. 

<img width="2716" height="358" alt="image" src="https://github.com/user-attachments/assets/2a0ab8ba-3fcf-4bdf-8b42-9dcd2b628582" />

## Standard Environment Variables 
Standard environment variables give us insight into various aspects of the system, the user and the runtime environment. They provide useful information that can help us create more adaptable Bash scripts.

In the example below I used standard environment variables. The output shows the result. 

- `$LOGNAME`: Outputs the Username.
- `$SHELL`: Outputs the default shell, in this case zsh.
- `$PWD`: Outputs the current working directory.
- `$PATH`: Outputs the directories that the shell searches to locate executable commands. 

<img width="2734" height="540" alt="image" src="https://github.com/user-attachments/assets/6c15d49f-2dad-4e25-97e8-184fc2ee38b3" />
