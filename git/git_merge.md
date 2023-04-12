1. `git merge <branch name` -> merges the branch to the feature branch, it creates a commit of merge, everytime you merge the branches.

2. `git rebase <branch name>` -> more cleaner way to merge two branches together, it will create a copy of feature infront of master, and actually copy our changes there, and moves the master to tip of copied feature branch. All branch commits will be copied infront of master, and there is a way to squash all the commits to a single commit, so only one one commit will be there.

3. `squash` -> merging multiple things in one.

4. `git rebase --interactive master` -> Interactive mode will create a commit. Inside that commit it will list all the commits of a branch. All branch commits will be copied infront of master, and this is a way to squash all the commits to a single commit, so only one one commit will be there.

5. `git pull <remote name> <branch name>` -> downloads all of the content and fast-forwards to merge with local, in case there are changes in the remote repo. It actually downloads the code of the following branch, and in whatever branch we are downloading it inside, it will actually merge that piece of code. If it can merge with a fast forward stratergy, it will merge without creating the merge commit, otherwise if our master(branch) has also moved forward, and the remote branch (created from same branch master in this case) has also moved forward, it will download and create a merge commit out of it.

6. `git fetch <remote name> <branch name> ` -> it just downloads the code from the branch, and does not merge it with master(local branch).

7. `cherry pick` -> pick a set of commits and add only that commits, instead of adding all the commits.

8. `git cherry-pick commit-id` -> this creats a new commit, but it creates a new commit on master with the message which is similar to that particular commit. Like if, there is a commit on feature branch, and we want to check/alter/dubug that particular commit, then this commands adds makes the same commit on master/main branch. And now this commit becomes a part of master branch.
