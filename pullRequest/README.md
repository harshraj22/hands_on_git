# What to do :
 
 * Create a new [issue](https://github.com/harshraj22/hands_on_git/issues) notifying other contributors about the work you are doing locally (so that two people don't do same thing), and wait until some maintainer approves your idea.
 * Create a new branch and switch to it ```git checkout -b <branch name> ```
 * Make changes and add those changes using ```git add *```. You may want to add only specific changes to be commited. In that case, write the full/relative path of files to be added.
 * Commit changes with a meaningful commit message using ```git commit -m "<your commit message>"```
 * Fetch and merge any changes from remote repo to your branch using ``` git pull upstream master ``` and manually merge conflicts if any (though there should not be any conflicts at this stage).
 * Finally push your local changes (along with your local branch to the remote repo) using ```git push -u origin <branch name> ```

Go to website and make a pr and reference the issue.
 * The maintainer is expected to merge once the issue has been referenced.

### Further reading 
Link for further reading about pull request