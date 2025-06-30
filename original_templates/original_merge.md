This task will help you experience what a Git merge conflict looks like — and how to resolve it.  

Steps:  

1. Make sure your local repo is up to date:  
    ```console
    git checkout main
    git pull  
    ```
3. Create a new branch:  
    ```console
    git checkout -b your-name-conflict
    ```
5. In this file, change the line below to something new.  
    ```
    > Original sentence:  
    > "This sentence will be changed in main to create a conflict."
    ```
6. Save, then commit and push:  
    ```console
    git add .
    git commit -m "Edit line for conflict practice"
    git push origin your-name-conflict
    ```
8. Go to GitHub and open a pull request.  

-----------------------------
STOP! Before Merging...
-----------------------------

6. Now switch back to main:  
    ```console
   git checkout main
    ```
8. Edit the SAME line to something DIFFERENT, then save and commit:  
    ```console
    git add merge_conflict.txt
    git commit -m "Change same line on main"
    ```
10. Pull just in case:  
    ```console
    git pull
    ```
-----------------------------
MERGE & RESOLVE
-----------------------------

9. Make sure you are back in main  
    ```console
    git branch
    ```
10. Use the command  
    ```console
    git merge [name of other branch]
    ```
12. Open the merge conflict resolver in VSCode  

13. Accept changes on each side as needed and complete the merge  

14. Check to make sure the feature branch can be deleted using  
    ```console
    git branch --merged
    ```
If it appears in the list, it can be deleted  

Now the feature branch is able to be deleted  
