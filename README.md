# GitNotes

##GIT BRANCH

###List all of the branches in your repository.
git branch --list

###Create a new branch called ＜branch＞
git branch <branch>

###Delete the specified branch. This is a “safe” operation in that Git prevents you from deleting the branch if it has unmerged changes.
git branch -d <branch>

###Force delete the specified branch, even if it has unmerged changes. This is the command to use if you want to permanently throw away all of the commits associated with a particular line of development.
git branch -D <branch>

###Rename the current branch to ＜branch＞.
git branch -m <branch>

## GIT FILE DIFFERENCE
###see file diff
git diff


##GIT STASH
###create new temporary stash
git stash save "Worked on stash function"

###see the list of stash created.
git stash list

###apply the selected stash. Stash history is not deleted.
git stash apply stash@{0}

###apply changes from top stash. Top stash history automatically deleted.
git stash pop

###remove the selected stash created.
git stash drop stash@{0}

###deletes all stash created.
git stash clear



##GIT CHECKOUT BRANCH
###Switched to branch <branchname>
git checkout <branchname>

###Simultaneously creates and checks out ＜new-branch＞. The -b option is a convenience flag that tells Git to run git branch before running
git checkout -b ＜new-branch＞


##GIT CHECKOUT FILE
###undo single file
git checkout -- <filename>

###undo all the file
git checkout -- .



###undo commited changes
git log 
git revert <paste commit id>
git revert -n <paste commit id>

###git reset 
git log
git reset --hard <paste commit id>




Reference:
https://www.bing.com/videos/search?q=git+revert+commit&docid=607989673921690192&mid=D41C72A90AA634BD364FD41C72A90AA634BD364F&view=detail&FORM=VIRE
Git Tutorial 5: Undoing/Reverting/Resetting code changes


GIT HUB DOCS
https://docs.github.com/en/repositories/creating-and-managing-repositories/deleting-a-repository
