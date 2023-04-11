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
