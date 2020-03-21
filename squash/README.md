# What to do :
Squash is used to convert (or join) multiple commits into a single commit.
  * Make a new branch and switch to it using the command ``` git checkout -b <branch name> ```
  * Make multiple commits (change ```- [ ] Change? ```) one by one and keep on commiting.
  * This should create 3 commits in your branch (confirm using ```git log --oneline```) and when you do a pull request, this should be shown as 3 individual commit.
  * Run ``` git rebase -i HEAD~4 ``` (rebase in interactive mode using last 4 commits) to squash commits. This opens up an editor with various options (hopefully it opened the editor you had set up earlier).
  * To squash commits, replace the word ```pick``` with ```squash```. The commit being sqashed won't be shown in ```git log``` and all changes will be mergwd with another commit.  (Follow the given links for better understanding)
  * Finally pull the upstream and push your changes.
  * The maintainer is then expected to merge the branch.

### Further Reading :

