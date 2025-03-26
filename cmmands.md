Git Commands Explanation

Initial Setup

ubuntu@ip-172-31-92-81:~$ git --version

Displays the installed Git version.

ubuntu@ip-172-31-92-81:~$ pwd

Prints the current working directory.

ubuntu@ip-172-31-92-81:~$ mkdir git-tutorial

Creates a new directory named git-tutorial.

ubuntu@ip-172-31-92-81:~$ cd git-tutorial/

Navigates into the git-tutorial directory.

Git Initialization

ubuntu@ip-172-31-92-81:~/git-tutorial$ git init

Initializes a new Git repository in the current directory.

ubuntu@ip-172-31-92-81:~/git-tutorial$ ls -la

Lists all files, including hidden ones (.git directory).

Creating and Tracking Files

ubuntu@ip-172-31-92-81:~/git-tutorial$ touch nibba.txt nibbi.txt

Creates two new empty files: nibba.txt and nibbi.txt.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git status

Displays the status of the repository, showing untracked files.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git add nibbi.txt

Adds nibbi.txt to the staging area.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git commit -m "adding nibba nibbi"

Commits the staged files with a message.

Removing Files and Restoring Changes

ubuntu@ip-172-31-92-81:~/git-tutorial$ rm nibbi.txt

Deletes nibbi.txt from the working directory.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git restore nibbi.txt

Restores nibbi.txt from the last committed state.

Configuring User Details

ubuntu@ip-172-31-92-81:~/git-tutorial$ git config --global user.name "<vibhavarisaraf4555>"

Sets the global Git username.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git config --global user.email "<vibhavarisaraf5444@gmail.com>"

Sets the global Git email.

Branching and Switching

ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout -b dev

Creates and switches to a new branch dev.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout master

Switches back to the master branch.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout -b from-dev

Creates and switches to a new branch from-dev.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git checkout -b from-master

Creates and switches to a new branch from-master.

Viewing Logs

ubuntu@ip-172-31-92-81:~/git-tutorial$ git log

Displays the commit history.

ubuntu@ip-172-31-92-81:~/git-tutorial$ git log --oneline

Displays the commit history in a concise format.

Summary

This document provides an explanation of all Git commands executed during the session, including initialization, adding files, committing changes, restoring files, configuring user details, creating branches, and checking logs.

