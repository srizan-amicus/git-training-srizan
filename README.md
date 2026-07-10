# git-training-srizan
Name:- Srizan Obed Singh
Training batch:- 2026
Date:- 09-July-2026

# Project Description
All about git fundamentals and advanced features, implemented in a real time project with practical use cases.

# Git Log

git log -oneline --graph 
 Used this command and it showed commit history in graphical format, It showed
Commit hash, commit message and Branch structure

git diff HEAD~2 HEAD
 used this command and it compared the current commit with 2 commits above this commit.

 made an update in the readme
 

 A Quick fix while stash exists

 # Git rebase Demo
 Added a line just for rebase demo, commit-1 

 REBASE demo - commit 2

 REBASE demo - commit 3

 REBASE demo - commit 4

 REBASE demo -  commit 5


removed a few minor changes for task 17

# Analysis for git blame
I used git blame on readme which is the most frequently modified file in this repository. The command identified the commit responsible for each line in the file. This made it easier to trace specific changes. It also made it easy to track changes.

In a Team project, git blame helps devs to understand code ownership and change history. If a bug appearsin a particular line, devs can quickly identify the commits that introduced the change. This simplifies debugging, code reviews and maintainence 

For example
- 3a9221c9  REBASE demo - commit 3
- 578b0f96  A Quick fix while stash exists