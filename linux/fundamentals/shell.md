# Linux Shell

A shell is a program that allows users to interact with a Linux operating system by entering commands.

Commands can be entered into the shell to perform tasks such as creating files and directories, navigating the filesystem and managing users and permissions.

## Bash

One of the most commonly used Linux shells is Bash, which stands for Bourne Again Shell.

I have been using Bash while practising Linux commands in Killercoda.

The following command can be used to check the current shell:

echo $SHELL

For example:

/bin/bash

This indicates that Bash is the current shell.

## Running Commands

The shell allows commands to be entered and executed.

For example:

`pwd`

The shell runs the `pwd` command and displays the current working directory.

Other commands I have practised include:

`ls`
`cd`
`mkdir`
`touch`
`cat`
`chmod`
`chown`

## Shell Environment

The shell also provides access to environment variables.

For example:

echo $SHELL

displays the path of the current shell.

## Practical Example

<img width="644" height="264" alt="image" src="https://github.com/user-attachments/assets/e6544794-a19d-4bbf-8aa0-d301cfd3baec" />

- I first used `echo $SHELL` to check the current shell which showed /bin/bash. This showed bash was the current shell.
- I then used `echo $0` and this returned bash
- I used bash --version to check the version of bash and it showed that I was using Bash version 5.2.21.
- I then used basic Linux commands like `pwd` which showed my current working directory `/root` and `ls` to list the content of the directory `filesystem`. 
