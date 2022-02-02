# learn-to-git  

#### Pushes to origin and track the branch  

        git push -u origin <branch>

#### Push to local branch as specified remote branch  

        git push origin <lbranch> : <rbranch>  

#### Removes remote branch permanantly, pushes nothing

        git push origin : <rbranch>  

#### Stash uncommitted work safely and lets you to goto some other branch  

        git stash list  
        git stash show -u # untracked  
        git stash drop <stash>  
        git stash pop <stash>  
        git stash push # pushes to head  
        git stash branch <branch> <stash>  

#### To be merged into current branch  

        git merge <branch to be merged>  

#### Squashes all commits into one commit  into the current branch

        git merge --squash <branch to be merged>

#### Changes tail/base of current branch to the specified commit/branch head *only if it finds change in ref*

        git rebase <branch/commit>  

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

#### Removes pathspec from staged  

        git restore --source= <of commit> --staged <pathspec> 

#### Restore un staged commits

        git restore <pathspec>

#### Swith branch and pull  

        git checkout <branch>

#### Re-writes modified code from origin

        git checkout  

#### Re-writes modefied file from origin  

        git checkout <pathspec>  

#### Creates and switches to the branch  

        git checkout -b <branch> 
