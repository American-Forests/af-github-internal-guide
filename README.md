# The American Forests Github Guide

A comprehensive guide on how to use and contribute to our organizational github! If you have any questions, please reach out to [Chase] (mailto:cdawson@americanforests.org).

## Why Github?

- version control is wonderful for reverting back to a working piece of code/script.
- back ups are excellent in the case of computer crashes or other sudden life events that mean you lose access to your computer
- it helps create visibility on who is working on which projects 

## Installing and Configuring Git (windows machines)
1. Download git from [git-scm.com](https://git-scm.com/download/win).
2. Run through the standard installation process
3. Open up the github bash terminal and run `ssh-keygen` to generate your public and private keys. (make sure to name them id_rsa)
5. Run ``eval `ssh-agent -s` `` followed by `ssh-add /d/Users/<username>/.ssh/id_rsa`
6. Run `cat /d/Users/<username>/.ssh/id_rsa.pub` and copy the output to your clip board. Then, add this to your github account in settings (NOTE: you might use `/c/` for some machines)

## Setting up a github repository
1. Create a repository online through the AF organization on github.
1. Navigate to your desired folder using `cd` and `ls`/`dir` commands.
2. Run `git init` to create a git repository for the appropriate folder.
3. Set up a `.gitignore` file to ignore all of the data/directories you want to 
4. For each file you want to back up to github, run `git add <relative file path>`.
5. Once you have added all the necessary files, run `git commit -m 'initial commit'`.
6. Then run `git branch -b main` to set the default branch to the main branch.
7. Next, run `git remote set-url git@github.com/American-Forests/<repo-name>.git` (ensure that you have already made the appropriate repo on github already)
8. Finally, run `git push --set-upstream origin main`.

## Backing up code
1. Run `git status` to check what changes you have made
2. Run `git add <relative file path>` for the files you have modified and want to back up. Alternatively, you can run `git add .` to back up all files.
3. Run `git commit -m "<commit message>"` to form a commit
4. Run `git push` to back up your code to the main branch!
