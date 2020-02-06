# What to do :
 * Swich to the branch that you created using ```git checkout <branch name>``` If you are already on that branch, it won't affect.
 * Make some changes
    ```- [ ] Change1 ``` to ``` - [x] Change1 ```
 * Add and commit the change. See [pullRequest](https://github.com/harshraj22/hands_on_git/tree/master/pullRequest) if you forgot.
 * Push the commit to remote repo using ``` git push ```
 * The maintainer is then expected to make some changes (preferably adding an extra space in the line where change is made) in your file in the master branch in order to make some conflicts in your pull request.
 * Do ``` git pull upstream master ``` to include all changes in the original remote master branch into your local branch.
 * Now you might find message saying conflict in the file that you created. ``` More Details will be added as why this happens, for now you may understand it as you made changes at same place where changes were made in master branch ```
 * Open the file in editor and edit/update changes in it. Now the file contains only the lines that you wanted.
 * Finally add, commit and push the commit. Your pull request will be updated with the latest commit.
 * Now the maintainer is expected to merge this pull request

### Further Reading :
