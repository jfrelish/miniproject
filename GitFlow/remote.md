# Remote

## What is git remote?

* The git remote command is one piece of the braoder system which is responsible for syncing changes.
* Manages set of tracked repositories

![Remote](/Images/Remote.PNG)

* User can [push](https://github.com/jfrelish/miniproject/blob/gitFlow/GitFlow/push.md) or [pull](https://github.com/jfrelish/miniproject/blob/gitFlow/GitFlow/pull.md) to rempte [repositories](https://github.com/jfrelish/miniproject/blob/gitFlow/GitFlow/repo.md)

### Add a remote repoistory

* To add a remote repoistory to your project, user would run the following command:
	* git remote add REMOTE-NAME REMOTE-URL
* The REMOTE-URL can be either HTTPS or SSH. User can find the URL on GitHub by clicking the "Clone or download" dropdown in their repository

![CloneDownload](/Images/CloneDownload.PNG)

* For example, if user want to add a remote repository and call it example, they would run:
	* git remote add example https://example.org/my-repo.git

### Remove a remote repository

* Using the -rm command will remove the remote named <name>. All remote-tracking branches and configuration settings for the remote will be removed.

* The syntax command is:
	* git remote rm REMOTE-NAME
* User can confirm the remote is gone by viewing the list of their existing remotes:
	* git remote -v

### Show a remote repository

* show command gives information about the remote repository

* With -n option, the remote heads are not queried first with *git ls-remote* repository; cached information is used instead.


