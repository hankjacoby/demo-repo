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

ls - shows all contents of current directory  
cat - shows the contents of specified file as they appear on the website  
pwd - prints the working directory  
cd - changes the directory being worked in  
vim - used as a different text-editor **use if comfortable  
git branch --merged - shows which branches have already been merged  
git branch -D [name of branch] - force deletes a branch even if its contents are not merged yet  
git diff [other branch] - shows all the differences in each file between the 2 branches  
git checkout [name of branch] - switches to that branch  
git branch - shows which branch you are currently working on  
