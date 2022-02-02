# learn-to-git  

### Commit  

#### Add changes to last commit again

        git commit --amend --no-edit

### Push

#### Push to remote forcebly by re-creating the commit or branch

        git push --force

#### Push all the private tags to remote

        git push --tags

#### Push all the private annotated tags to remote

        git push --follow-tags

#### Pushes to origin and track the branch  

        git push -u origin <branch>

#### Push to local branch as specified remote branch  

        git push origin <lbranch> : <rbranch>  

#### Removes remote branch permanantly, pushes nothing

        git push origin : <rbranch>  

### Stash  

### uncommitted work safely and lets you to goto some other branch  

        git stash list  
        git stash show -u # untracked  
        git stash drop <stash>  
        git stash pop <stash>  
        git stash push # pushes to head  
        git stash branch <branch> <stash>  

### merge

#### To be merged into current branch  

        git merge <branch to be merged>  

#### Squashes all commits into one commit  into the current branch

        git merge --squash <branch to be merged>


### Rebase  

#### Changes tail/base of current branch to the specified commit/branch head *only if it finds change in ref*

        git rebase <branch/commit>  

### Reset  

#### Resets head to speacific commit  

        git reset <commit>  

#### Reset pathspec from staged  

        git reset <pathspec> 

#### Changes head to the commit, index, working tree # all changes will be lost  

        git reset --hard <commit> 

#### Changes head to commit, index but not workingg tree; git status report changes

        git reset --mixed <commit>  

#### Changes head to commit, but wont touch index and working tree; git status stilll recognize changes  

        git reset --soft <commit>  

### Restore

#### Removes pathspec from staged  

        git restore --source= <of commit> --staged <pathspec> 

#### Restore un staged commits

        git restore <pathspec>

### Revert

#### fetches contents of the commit specified and creates new commit  

        git revert --edit <commit>
        git revert --no-edit <commit>
        git revert --no-commit <commit>

### Checkout

#### Swith branch and pull  

        git checkout <branch>

#### Re-writes modified code from origin

        git checkout  

#### Re-writes modefied file from origin  

        git checkout <pathspec>  

#### Creates and switches to the branch  

        git checkout -b <branch> 

### Tag

#### Create tag  

        git tag  <tag> 

#### Create annotated tag  

        git tag -a -m "message" <tag> 

### Status

#### Shows the status of the git

        git status

### Log

#### Shows the git log; commit by commit

        git log
        git log --oneline
        git log --grep <patten>
