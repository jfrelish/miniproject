# Pull

* git pull is a Git command used to update the locak version of a repository from a remote.

#### Example of the git pull

![Pull](/Images/Pull.PNG)

* git pull is one of the four commands that prompts network interaction by Git. By default, git pull does two things.

	1. Updates the current local working branch (checkout branch)
	2. Updates the remote tracking branches for all other branches.

* git ull fetches (git fetch) the new commits and merges ([git merge](https://github.com/jfrelish/miniproject/blob/gitFlow/GitFlow/merge.md)) these into your local branch.

![Pull2](/Images/Pull2.PNG)

in which:

* OPTIONS are the command options, such as --quiet or --verbose. You can read more about the different options in the Git documentation
* REPOSITORY is the URL to your repo. Example: https://github.com/freeCodeCamp/freeCodeCamp.git
* REFSPEC specifies which refs to fetch and which local refs to update
* REMOTE-NAME is the name of your remote repository. For example: origin.
* BRANCH-NAME is the name of your branch. For example: develop.

[Reference](https://guide.freecodecamp.org/git/git-pull/)
