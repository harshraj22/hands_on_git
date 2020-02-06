# What to do :
Squash is used to convert (or join) multiple commits into a single commit.
 * Make a new branch and switch to it using the command ``` git checkout -b <branch name> ```
 * Make multiple commits (change ```- [ ] Change? ```) one by one and keep on commiting.
 * This should create 3 commits in your branch and when you do a pull request, this should be shown as 3 individual commit.
 * Run ``` git rebase -i HEAD~4 ``` to squash commits. (Follow the given links for better understanding)
 * Finally pull the upstream and push your changes.

### Further Reading :
