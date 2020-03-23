# For various How To's done in daily work.

#### I hate git ! How to get rid of this tracking without loosing my work ?
- ```rm -rf .git``` (make sure you are in same directory in which .git is present)

#### How to set autocompletion (on hitting tab) in git ?
- ```git config --global help.autocorrect 1```

#### See log in better way.
- ```git log --oneline --graph```

#### How to remove each changes made to a file since last commit (the file isn't added to staging area) ?
- ```git checkout -- <filename>```

#### How to undo git add (remove a file from staging area) ? 
- ```git reset HEAD -- <filename>```

#### I commited a file. How to remove it from commit ?
- ```git reset --soft HEAD~1``` , This brings back all changed/created/deleted files in last commit to staging area.

#### I want to pull upstream accepting all incoming changes in case of merge conflict.
- ```git pull -X theirs``` [source](https://stackoverflow.com/questions/10697463/resolve-git-merge-conflicts-in-favor-of-their-changes-during-a-pull)

#### How to checkout to a pull request branch locally ?
- ```git fetch upstream pull/<ID>/head:<BRANCHNAME>``` . ID is the pull request id (headed by a # in pull request) and BRANCHNAME is some random name to newly created local branch. If pull request is made on origin, use origin instead of upstream.

#### How to delete a remote branch created by me locally ?
- ```git push origin --delete <branchname>```

#### I commited some files earlier. Now I want to add them to .gitignore, how to forget them being tracked ?
- first add and commit .gitignore, then - ```git rm --cached <path-to-file>``` and then ```git add .``` [source](https://stackoverflow.com/questions/1274057/how-to-make-git-forget-about-a-file-that-was-tracked-but-is-now-in-gitignore)

#### How to check all changes to a file ?
- This is where you understand the value of good commit messages. use ```git log -p --name-only --oneline  <filename>```
##### Find more on [this repo](https://github.com/git-tips/tips)