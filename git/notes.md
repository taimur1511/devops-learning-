## How does Git work? 

Working Directory - This is where you edit your file and make changes

Staging Area - This is where you put files that you want to commit 

Repository - Local Git folder. Once you are on Git commit your files go from the staging area to your repository. 

Flow: 

[Working Directory] > git add > [Staging Area] > git commit > [Repository]. 

## Essential Git Commands 

`git init` - Initialises a new Git repository.

`git status` - Shows the current state of your working directory.

`git add .` - Stages all changes ready to be committed.

`git commit -m "message"` - Saves staged changes with a descriptive message.

`git log` - Displays the commit history.

`git diff` - Shows changes made to files.

`git branch` - Lists your existing branches.

`git switch -c <name>` - Creates and switches to a new branch.

`git switch <name>` - Switches to an existing branch.

`git merge <branch>` - Merges another branch into your current branch.

`git restore <file>` - Discards unstaged changes to a file.

`git stash` - Temporarily saves uncommitted changes.

`git stash pop` - Restores your stashed changes.

`git revert <commit>` - Creates a new commit to undo an earlier commit.
