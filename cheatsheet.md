### Cheatsheet
```
# Clone a repo
$ git clone REPO_NAME

# Fetch the state of your local repository
$ git status

# Promote the change to the staging area
$ git add FILE_NAME/DIRECTORY_NAME

# Commit the change in the staging area
$ git commit

# History of change/history of commits
$ git log

# Upload the committed change to the remote repository
$ git push

# Initialize git repo locally
$ git init

# Add remote repo
$ git remote add origin URL_OF_REMOTE_REPO

# Push to the remote repo for the first time
$ git push --set-upstream origin master

# List available branch
$ git branch

# Pulling the latest code from the remote repo (git fetch + git merge = git pull)
$ git pull

# Switching branch
$ git checkout BRANCH_NAME

# Create a new branch locally base from master branch
$ git checkout master
$ git checkout -b BRANCH_NAME

#
$ git push --set-upstream origin LOCAL_BRANCH_NAME

# Delete local branch
$ git checkout master
$ git pull
$ git branch -d BRANCH_NAME_TO_DELETE

# Pull vs Pull Rebase (merge branch commit)
$ git pull --rebase

#
$ git stash
$ git stash pop

# Going back in history
$ git log
$ git checkout COMMIT_HASH

# Undo commit by discarding it and its changes
$ # MAKE THE CHANGE THEN COMMIT
$ git reset --hard HEAD~1

# Undo a commit by discarding it but its changes will be brought back to the pre-staging area
$ # MAKE THE CHANGE THEN COMMIT
$ git reset --soft HEAD~1

# Commit the changes to the last commit. Or introduce a change to the last commit without discarding it.
$ # MAKE THE CHANGE THEN COMMIT
$ git commit --amend

# Undo commit that was pushed for Merge/Pull Request
$ # PUSH THE COMMIT
$ git reset --hard HEAD~1
$ git push --force

#
$ git revert COMMIT_HASH

# Pulling changes from the updated master local branch to your WIP branch
$ git checkout master
$ git pull
$ git checkout WIP_BRANCH
$ git merge master
```

