This file will be modified several times to simulate mistakes.

In this task, you'll learn how to undo previous commits using their Git hashes
with both 'revert' and 'reset'.

You'll make three commits, push them, then undo the second one in two different ways.

Steps: 

1. Make sure you are on a new branch
    ```console
    > git checkout -b undo_branch
    ```
2. Open undo_commit.txt and add a line at the bottom

3. Stage and commit the new change

    > git add .
    > git commit -m "first good commit"

4. Add a second line below the one you just made

5. Commit that change too, we will treat this commit as the mistake

    > git add .
    > git commit -m "mistaken change"

6. Add a third line just like steps 2 and 4

7. Commit the new change

    > git add .
    > git commit -m "another good change"

8. Push the changes

    > git push origin undo_branch

9. View the log to see the last few commits

    > git log

10. Find the hash value of the mistaken commit

    Each entry here is in reverse chronological order
    It will look something like this

    commit [hash_value]
    Author: [user] <user_email>
    Date: [day_of_week] [month] [day_of_month] [time]

        [commit_message]

    This is why commit messages are more important than originally let on
    Commit messages are useful to identify the right commit to return back to

Continuing from here there are three ways to undo, which is why there will be three
sets of instructions from here on out. The first way is safe, the second is unsafe, 
and the third is a shorthand that skips the hash values and can be done using either
the first or second method.

Option 1 (Safe) - using git revert

11. Revert back to the change we want to undo

    > git revert [hash_value]

12. After dealing with the error in the merge conflict resolver,
    this creates a new commit that undoes that change

13. Push this new version

    > git push

This option makes a new commit undoing these changes
while keeping the commit history intact!

Option 2 (Unsafe) - using git reset with the hash

11. Reset the branch

    > git reset --hard [hash_of_commit_before_mistake]

12. Force the branch to accept these changes

    > git push --force

This option overwrites the commit history on GitHub!

I also want to show a shorthand version that does not
require the hash, as long as you keep a good mental history
of the commits in your head. The following shorthand method
works for both revert and reset, but I will use reset for
this demonstration.

11. To undo two commits, run this command

    > git reset --hard HEAD~2

    Here the hard flag moves the HEAD (pointer to latest commit)
    back 2 commits (specified after the tilde), and discards all the changes, 
    including files in the folder. Using the soft flag would move the HEAD back 
    but keeps all the changes staged. The default behavior is the mixed flag, 
    which moves the HEAD back and unstages the changes.

12. Then force the changes onto the repository

    > git push --force

Hank never makes mistakes
