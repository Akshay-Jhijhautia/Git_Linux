1. `git merge <branch name` -> merges the branch to the feature branch, it creates a commit of merge, everytime you merge the branches.

2. `git rebase <branch name>` -> more cleaner way to merge two branches together, it will create a copy of feature infront of master, and actually copy our changes there, and moves the master to tip of copied feature branch. All branch commits will be copied infront of master, and there is a way to squash all the commits to a single commit, so only one one commit will be there.

3. `squash` -> merging multiple things in one.

4. `git rebase --interactive master` -> Interactive mode will create a commit. Inside that commit it will list all the commits of a branch. All branch commits will be copied infront of master, and this is a way to squash all the commits to a single commit, so only one one commit will be there.

5. `git fetch --all` ->

6. `git pull --all` ->
