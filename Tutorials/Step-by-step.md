
# **_Git setup tutorial_**:


 ***step 1:*** Setup a Github account at [gitHub](https://github.com) and make your very own repository
 
 
 **step 2:** Download, install and run git [git](https://git-scm.com/downloads) 
 
 
 **step 3:** Run GIT and generate a key using the command $ ssh-keygen -t rsa
 
 
 **step 4:** When it asks to enter a file to save it into; hit enter. It willthen ask you for a paraphrase, hit enter again.
 
 
 **step 5:** At this time, you have generated a key and stored it, the next thing is to find it and store it into github
 
 
 **Step 6:** To find the actual key type in $ cat~/ .ssh/id_rsa.pub, copy the key and head on over to your github profile.
 
 
 **Step 6A:** Another alternate way to generate the key is explained [here](https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent)
 
 
 **Step 7:** Once at [gitHub](https://github.com) click on the top right and navigate to settings.
 
 
 **Step 8:** Click on the tab to the left that says SSH, from there paste your key onto the SSH box.


## Collaborative work:


_Got friends who would like to work on the repository as well, why not add them as collaborators?!_



**Step 1:** Request for Collaborators username


**Step 2:** Navigate to [gitHub](https://github.com) and click on the repository that you have made earlier.


**Step 3:** Select the settings tab under your repository name. 


**Step 4:** Click on 'Collaborator' option


**Step 5:** Inside the Collaborators option, add in the username of the collaborators that you wish to work with.


**Step 6:** Click on 'Add Collaborator' button


**Step 7:** Wait for acceptance.


# Forking vs cloning


### What is cloning? 


Cloning is the process of copying or downloading a repository onto GIT Terminal, assuming that you have write access, you are able to push any changes to the direct repository. 
[Read More >](/Forking-Vs-Cloning/cloning.md)

### What is forking? 


Forking is the process of copying a repository onto your own Github account, with this you are able to make any changes you want without affecting the original repository.
[Read More >](/Forking-Vs-Cloning/forking.md)




### Pull Request

Pull Request are request to the original Repository owner and sends them a notification that you want a branch or section that you worked on to be merged onto the original repository. The owner will then review the pull request and either accept of deny the request.



# Branching

After adding your friends as collaborators, branching from the master branch is the best way for you or other collaborators to work in harmony without affecting the master branch unless you Merge your work into master. Branching off from the master branch avoids a merge conflict since the collaborators are not doing their work on the master branch  


**step 1:** Open Git and type the following command: cd your-repository-name


**step 2:** make sure to update the local repository with the command: git pull


**step 3:** To branch off from master type in git checkout -b <branch-name-goes-here>; this command will make a new branch and checkit out. At this point you should be on your newbranch.


**step 4:** You need to push these changes to the remote repository with the command git push origin <new-branch-name>


![](https://github.com/jfrelish/miniproject/blob/school/Pictures/Screenshot%20(17).png)

Merge conflicts happens in GIT when it cannot automatically resolve the differences between two commits.

# Merge conflict illustration.


![](https://github.com/jfrelish/miniproject/blob/school/Pictures/merge%20conflict%201.png)


![](https://github.com/jfrelish/miniproject/blob/school/Pictures/merge%20conflict%202.png)






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
