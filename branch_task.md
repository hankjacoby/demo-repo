In this exercise, you will learn how to make new branches, and merge them back into the main branch  

Your task:  

1. Create a new branch:  
    ```console
    git checkout -b your-name-branch
    ```
    **checkout - to switch to a new branch  
    **-b (flag) - makes a new branch  

2. Add a new note to the file at the bottom  

3. Commit and push using these 3 commands  
    **Note: Make sure to Ctrl + S to save the file in VSCode before attempting to add  
    ```console
    git add . 
    ```
    **using the period adds all modifications to be staged, if you want you can specify a file instead  
    *add - adds the file(s) changed as staged changes (ready to commit)  
    ```console
    git commit -m "Added idea by [Your name]"
    ```
    **commit - saves the file changes to be pushed  
    **-m (flag) - specifies the message to be used for the push request  
    ```console
    git push origin your-name-branch
    ```
    push - pushes the staged changes to the group's repository for all to see

4. Go to the GitHub website and open a pull request (PR)  

**Note: Do not merge blindly, always make sure to go through the changes  
        to make sure that we aren't losing functionality  

5. Merge it into main after reviewing  

6. Change back to main and clean up the tree in VSCode terminal  
    ```console
    git checkout main

    git pull 

    git branch -d [name_of_branch]
    ```
    **-d (flag) - this deletes the branch if already merged

Useful Tip: 
Use the command below to see a list of all the branches as well  
as to see what branch you are currently working in  

```console
git branch
```

Add your note below
