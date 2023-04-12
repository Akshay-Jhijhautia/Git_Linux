1. `git reset` -> git reset not only moves head pointer but also master(branch) pointer. It has 3 modes - 1. soft mode 2. mixed mode 3. hard mode
2. `git reset --soft commit id` -> Both master(branch) and head will move to that particular commit. It does not make any changes to the staging area or the working directory(untracked files). But hard mode and mixed mode can make changes to your staging area and working area(untracked files).

3. `git reset ORIG_HEAD` -> to revert the changes of the point 2. It will point to last commit before reset. But if we do 2 or multiple resets, then this command will not work.

4. `git reset --soft HEAD~` -> will point the both head and branch to parent of head.

4a. `git reset --soft HEAD~2`
4b. `git reset --soft HEAD^`

5. `git reset --mixed HEAD~` -> it will move head and branch pointer to the parent commit,and any pending changes in the staging are reverted till that commit only. Changes after that commit are removed from staging area and moved to working area.

5a. `git reset --mixed commitid` -> moves the head and branch pointer to that particular commit, and any pending changes in the staging are reverted till that commit only. Changes after that commit are removed from staging area and moved to working area.

6. `git reset commit id` -> default it is mixed reset

7. `git reset --hard HEAD~` -> it will move the branch and head pointer to the parent commit. The staging area and the working area are reset to match that of the specified commit. Any previously pending changes to the staging area and the working area gets reset to match the state of the commit tree. This means any pending work that was hanging out in the staging are and working area will be lost. All changes pending in staging area and working area are deleted.

7a. `git reset --hard commit id` -> moves the head and branch pointer to that particular commit, and any pending changes in the staging area and working area are reverted till that commit only, ie. any changes made in the staging area or working area after that particular commit are deleted.

# Impotant points in short

a. Moving head and branch pointer
b. Reset the staging area
c. Reset the working area

`git reset --soft commitid` -> a
`git reset --mixed commitid` -> a & b
`git reset --hard commitid` -> a & b & c

8. `git revert HEAD` -> This command is used for undoing changes to a repository's commit history.It will make a new commit with opposite changes of the last commit. It does not move any refenence pointers to that commit. It is a revert operation that will take a specified commit, inverse the changes from that commit, and create a new "revert commit". The reference pointers are then updated to point at the new revert commit making it the tip of the branch. It can revert changes of a commit, if we try to make changes to multiple commits, then it might create merge conflict.
