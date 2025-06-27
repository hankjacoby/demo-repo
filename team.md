This exercise is the first step in learning how to use Git and GitHub  
At this point, the repository should be cloned and ready to work with  

Steps: 

1. Add your name to a list of names at the bottom of this file below the Steps

2. Hit Ctrl + S to save the file in VSCode

3. Run these commands in the VSCode terminal
    ```console
    git add .
    ```
    This stages all the changes you've made to be committed later
    ```console
    git commit -m "YOUR MESSAGE HERE"
    ```
    This saves the changes ready to be added  
   ```console
    git push origin main
    ```
    Pushes the changes to the remote repository for all to see  
5. Reload the GitHub page to make sure your changes are reflected on the website, or
   use cat team.md to see the version GitHub has

Useful Tip: 

Add -u to the last command to set origin main as the upstream, meaning future push commands
won't have to specify main as the location if thats the intended path

Using this tip, that last command would look like this:
```console
git push -u origin main
```

Add name under here
