Your task:

1. Create a new branch:
    
    git checkout -b your-name-branch

    **checkout - to switch to a new branch
    **-b (flag) - makes a new branch

2. Add a new note to the file at the bottom like I have

3. Commit and push using these 3 commands
    **Note: Make sure to Ctrl + S to save the file in VSCode before attempting to add

    git add . 
    
    **use the period for all staging, can also specify files using their names
    *add - adds the file(s) changed as staged changes (ready to commit)

    git commit -m "Added idea by [Your name]"

    **commit - saves the file changes to be pushed
    **-m (flag) - specifies the message to be used for the push request
    
    git push origin your-name-branch

    push - pushes the staged changes to the group's repository for all to see

4. Go to GitHub and open a pull request (PR)

**Note: Do not merge blindly, always make sure to go through the changes 
        to make sure that we aren't losing functionality

5. Merge it into main after reviewing

6. Change back to main and clean up the tree in VSCode terminal

    git checkout main

    git pull 

    git branch -d [name_of_branch]

    **-d (flag) - this deletes the branch if already merged

Useful Tip: 
Use the command "git branch" to see a list of all the branches as well
as to see what branch you are currently working in

Hank Jacoby loves GitHub