# Push

* The git push command allows user to send (or push) the commits from user local branch in theur local Git repository to the remote repository.

![Push](/Images/Push.PNG)

* Command syntax is as follows:

	* git push <repo name> <branch name>

##### Push to a specific remote repository and All Branches in it

* If you want to push all your changes to the remote repository and all branhces in it, the command syntax is as follows:
	* git push --all <REMOTE-NAME>
	in which:
	* --all is the flag that signals that user want to push all branches to the remote repository
	*REMOTE-NAME is the name of the repository you want to push to

##### Push to a specific branch with force parameter

* If user want to ignore the local changes made to Git repository at GitHub then user can use -force command to push by ignoring those changes. 
	* git push --force <REMOTE-NAME><BRANCH-NAME>
	in which:
	* REMOTE-NAME is the the name of the repository to which user want to push the changes to
	*BRANCH-NAME is the name of the remote branch you want to push your changes to

[Reference](https://guide.freecodecamp.org/git/git-push)

