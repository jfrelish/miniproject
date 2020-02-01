
# Merge Conflicts


Merge conflicts happens in GIT when it cannot automatically resolve the differences between two commits.

# Merge conflict illustration.


![](/Images/merge%20conflict%201.png)


![](/Images/merge%20conflict%202.png)






# Merge Conflict Solution:



To resolve a merge conflict caused by competing line changes, you must choose which changes to incorporate from the different branches in a new commit.


For example, if you and another person both edited the file styleguide.md on the same lines in different branches of the same Git repository, you'll get a merge conflict error when you try to merge these branches. You must resolve this merge conflict with a new commit before you can merge these branches.


> Open Git Bash.


> Navigate into the local Git repository that has the merge conflict.


> cd REPOSITORY-NAME


Generate a list of the files affected by the merge conflict. In this example, the file styleguide.md has a merge conflict.
> $ git status
>  On branch branch-b
>  You have unmerged paths.
>    (fix conflicts and run "git commit")
> 
>  Unmerged paths:
>    (use "git add ..." to mark resolution)
> 
>  both modified:      styleguide.md
> 
> no changes added to commit (use "git add" and/or "git commit -a")


Open your favorite text editor, such as Atom, and navigate to the file that has merge conflicts.


To see the beginning of the merge conflict in your file, search the file for the conflict marker "<<<<<<<". When you open the file in your text editor, you'll see the changes from the HEAD or base branch after the line "<<<<<<< HEAD". Next, you'll see "=======", which divides your changes from the changes in the other branch, followed by ">>>>>>>" "BRANCH-NAME". 


Decide if you want to keep only your branch's changes, keep only the other branch's changes, or make a brand new change, which may incorporate changes from both branches. Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge. 


## Optional Conflict Resolution with vimdiff
After the warning about file CONFLICT, the comand `git mergetool` can be used to launch a visual editor to fix it. The screenshot shows 4 panels. The top row from from left to right is: OURS/local, base, THEIRS/remote. The single window at the bottom half of the screen is the output window, which is the resolved file which will be saved. 

![CloneDownload](/Images/Resolving_a_merge_conflict.PNG)

* [Helpful vim commands](https://vim.fandom.com/wiki/Copy,_cut_and_paste)
* [Vimdiff commands](https://gist.github.com/mattratleph/4026987)


# Add or stage your changes.


> $ git add .


> Commit your changes with a comment.


> $ git commit -m "Resolved merge conflict by incorporating both suggestions."


> You can now merge the branches on the command line or push your changes to your remote repository on GitHub and merge your changes in a pull request.
