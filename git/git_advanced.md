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

15. `git checkout commitid -- <file name->` -> If we do git checkout on a commit using a commit id, it will make copies to both working area and staging area from the corresponding commit, so whatever changes we have in that particular commit, those changes are going to come back. Checkout moves your head pointer.

Note: To revert back the changes, or to revert a particular file to its previous state, in such a case git checkout commands is really helpfull.

16. `git clean -f` -> it will clean the working area, by deleting the untracked files.

16a. `git clean --dry-run` -> will inform you of the files that will be deleted.

17. `git clean -d --dry-run` -> this will inform, what folders/directories will also get deleted.

18. `git clean -d -f` -> will remove untracked files and folders as well.

19. `git checkout commitid` -> it detaches head from the branch, instead head points to a particular commit.

20. `git switch -` -> it reverses the point 19, i.e. now head points to a particualar branch

21. `git log --since="yesterday`
22. `git log --since="5 minute ago`
23. `git log --grep=second` -> grep is used for pattern matching, it will return commit which has string "second" in it.
24. `git log --since="1.minute`
25. `git log --since="10.minute`
26. `git log commitid^n` -> it will give the nth parent of that particular commit.
27. `git log commitid~n` -> this will give us nth node/parent of that particular commit.
28. `git merge` -> it merges two branches, so one commit can have two heads/parents.
