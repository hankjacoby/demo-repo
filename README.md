# Git & GitHub Guide for Our Team

Welcome to our Git learning environment! This guide will help you understand how to use Git and GitHub to contribute to our project smoothly and confidently.

---

## Repositories Overview

- **demo-repo (sandbox):** Practice Git commands, make mistakes, and learn safely.
- **(unsure of name rn):** Our real project. All meaningful contributions will go here once you're comfortable.

---

## Setup Instructions

### 1. Install Git
The link below should guide you on how to download Git on your computer if you need to, no matter the OS.
[Link Here](https://www.atlassian.com/git/tutorials/install-git)

---

### 2. Sign up in GitHub

If you do not already have a GitHub account, please create one. Purdue or IU emails should allow for
better resources, however projects will be lost when
students no longer have access to those accounts if
they are not backed up with another email address.

### 3. Download VSCode (optional)

Downloading VSCode or any other IDE is not required,
you could technically only use the website or VIM, 
but I'd recommend downloading an IDE and connecting
your GitHub account to that IDE, for debugging and
linter purposes. This tutorial will also be written 
mostly for people using VSCode instead of another 
IDE or the HTTPS version.

### Maybe more to be added later

## Git Training Sandbox

Welcome to our dummy repository for learning Git and GitHub safely!

You’ll learn to:
  
  Clone a repo  
  Make commits  
  Push and pull  
  Create and merge branches  
  Resolve merge conflicts   

Follow each step below:

### 1. Clone the Repo

Run the commands below  

  > git clone https://github.com/hankjacoby/demo-repo  
  > cd demo-repo  

The first command clones the files to your machine, while
the second one changes directories into the repository

You can instead use the Command Palette in VS Code (Ctrl+Shift+P) and type Git: Clone, then paste the URL

### 2. Add yourself to team.txt

This first exercise is the first building block of using GitHub. This exersice teaches
you how to edit files and publish those changes safely. 
Follow the steps in the team.txt file to complete this learning task.

### 3. Complete the steps in branch_task_template.txt

This second exercise is another building block of using GitHub. This exercise teaches
you how to make branches, edit branches, and merge the changes back into main safely.
Follow the steps in the branch_task_template.txt to complete this learning task.

### 4. Complete the steps in merge_conflict.txt

This third exercise is another building block of using GitHub. When a merge conflict inevitably
occurs, this will teach you how to deal with them.
Follow the steps in the merge_conflict.txt file.

## Useful Commands to Know  
**Note: anything in square brackets [like_this] is an argument and should be replaced by you  

### Directory Navigation  

ls - shows all contents of current directory  
ls -la - shows all contents (including hidden files and folders) of the current directory  
cd [folder_name] - navigates into that folder  
cd .. - navigates to parent directory (like a back button)  
cd ~ - navigates to the home directory  
pwd - prints the working directory  
cat [file_name] - prints the contents of the specified file

### File Manipulation  

mkdir [folder_name] - makes an empty directory with the specified name  
touch [file_name] - makes an empty file with the specified name  
rm [file_name] - deletes the specified file  
mv [arg1] [arg2] - used to move a directory or file, or to rename a directory or file  
cp [file_1] [file_2] - copy the contents of file_1 into file_2  
less [file_name] - view the contents of a file with search and scroll  
wc -l [file_name] - counts the number of lines in a file  
echo "[message]" > [file_name] - replace the contents of file_name with message  
echo "[message]" >> [file_name] - append message to the end of file_name  

### Search and Compare

grep [message] file - searches for message in file  
diff [file_1] [file_2] - shows differences between file_1 and file_2  
sort [file_name] - sorts the lines of file_name in alphabetical order  
sort -n [file_name] - sorts the lines of file_name in numerical order  

### Git Commands

git status - shows stages, unstaged, and untracked files  
git diff - shows differences between working directory and index  
git diff --staged - shows differences between staged changes and last commit  
git log - view full git history  
git branch --merged - shows which branches have already been merged

### Git Branching

git branch - list local branches and specify current branch  
git branch -d [branch_name] - deletes the branch if merged  
git checkout [branch_name] - navigate to branch_name  
git checkout -b [branch_name] - creates a new branch with specified name  
git push origin --delete [branch_name] - deletes the branch from the website

### Git Commiting

git add [file_name] - stages the changes of that file  
git add . - stages all changes  
git commit -m "[message]" - commits changes with the message  
git restore [file_name] - undo changes to an unstaged file  

### Git Push and Pull

git pull - download and merge changes  
git push - add your changes to the remote repository  
git fetch - downloads updates without merging  
git push origin [branch_name] - pushes a branch to GitHub
