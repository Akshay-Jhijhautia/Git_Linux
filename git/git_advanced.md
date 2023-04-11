Note : Stash is maintained in LIFO way, like stack data structure. If we want to add a file to stash, then add that particular file by git add and then just do git stash.

1. `stash` -> stash are kind of safe case/locker, where we can save a bunch of uncommitted stuff. Let say, we did some changes to the code, and we do not want to commit the changes neither we want to discard the changes, in such cases we use stash.

2. `git stash` -> adds the file in stash

3. `git stash list` -> gives the list of files in the stash.

4. `git stash apply` -> whatever is the last stash will be applied, to bring back files from stash.

4a. `git stash apply@{1}` -> brings back a particular stash

5. `git stash show stash@{1}` -> to view/track changes done in the file stored in the stash.

6. `git stash --include-untracked` -> to save changes of untracked files

6a. `git stash save "<message>"--include-untracked`

7. `git stash pop` -> to apply the changes to stash and drop them

8. `git stash drop` -> to remove the stash without applying the changes to that stash.

9. `git stash clear` -> removes all the stashes

10. `git stash save "<message>"` -> to add a new message while stashing the file.

11. `git commit --amend` -> to change the files, without doing any further commits.

12. `fork` -> create a copy of repository in your own account

13. `upstream` -> upstream is from where you clone the repository, and downstream is any project that integrates your work with other works.

14. `git checkout --<filename>` -> If we do git checkout on a file, it will overwrite working area file with staging are file, so we will lose all of the changes, that was actually in the working area.

15. `git checkout 04fc18764255346a658940c998e08098d74eaf7e` -- <file name-> If we do git checkout on a commit using a commit id, it will make copies to both working area and staging area from the corresponding commit, so whatever changes we have in that particular commit, those changes are going to come back.

Note: To revert back the changes, or to revert a particular file to its previous state, in such a case git checkout commands is really helpfull.
