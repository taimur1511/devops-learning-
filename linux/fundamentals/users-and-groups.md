# Users and Groups 
Linux uses users and groups to manage access to files, directories and system resources.

## Users 
A user account represents an individual or service that can interact with a Linux system.

Each user has their own account and permissions.

## Creating a user

The `useradd` command can be used to create a new user.

`useradd` username

## Viewing users
The `/etc/passwd` file contains information about user accounts on the system.

The cat command can be used to view its contents:

`cat` /etc/passwd

## Groups
Groups are used to organise users and manage permissions.

A user can belong to one or more groups.

##Creating a group
The `groupadd` command can be used to create a new group.

`groupadd` groupname

## Adding a user to a group
The `usermod` command can be used to modify a users account. The `-aG` options can be used to add a user to an existing group.

`usermod -aG` groupname username

## Checking group membership

The `groups` command shows the groups that a user belongs to.

`groups` username

## Practical Example
I practised creating a new user and group using Killercoda.


