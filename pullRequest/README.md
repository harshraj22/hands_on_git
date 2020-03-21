# What to do :
 
 * Create a new [issue](https://github.com/harshraj22/hands_on_git/issues) notifying other contributors about the work you are doing locally (so that two people don't do same thing), and wait until some maintainer approves your idea. This is generally done by assigning issue to you.
 * Create a new branch and switch to it ```git checkout -b <branch name> ```. You may list all the existing local branches using ```git branch``` (the astrick ```*``` sign is on the current branch). Remember, the new branch contains local commits and untracted changes to files (red coloured files on running ```git status```) that your current branch contains (if any). Hence it is good idea to checkout to master (or develop if exists) to avoid any previous commits. Also in case there are any untracked changes, [stash](https://www.atlassian.com/git/tutorials/saving-changes/git-stash) them before checking out to other branch. Whenever you want to continue, you can apply those stash back easily.
 * Now since you have switched to a new branch (confirm by running ```git branch``` and check astrics) feel free to make changes to the files you wish. You won't mess up things in original repo from here.
 * Make suggested changes (fill your name in markdown file that you copied to the directory that you created) and add those changes using ```git add *```. This adds all files to staging area which have been changed/ created/ deleted. You may want to add only specific changes to be commited. In that case, write the full/relative path of files to be added in place of wildcard(*).
 * Commit changes with a meaningful commit message using ```git commit -m "<your commit message>"```
 * Fetch and merge any changes from remote repo to your branch using ``` git rebase upstream/master ``` and manually merge conflicts if any (though there should not be any conflicts at this stage). It is a very good practice to sync up your branch with remote head branch (may be other than master) before pushing your changes. Note that we used rebase for pulling changes from remote repo and merging to your current branch. More about rebasing will be covered later.
 * Finally push your local changes (along with your local branch to the remote repo) using ```git push -u origin <branch name> ```

Go to Github and make a [pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request) on master branch and [reference](https://help.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue) the issue.
 * The maintainer is expected to merge once the issue that you were assigned has been referenced.

### Further reading 
Link for further reading about pull request
