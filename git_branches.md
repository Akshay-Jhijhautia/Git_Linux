1. `branches` -> Technically branches are nothing but a, "Pointer to a particular commit".

2. `git checkout -b <name>` -> to create a branch, actually this command creates a new pointer to a particular commit. And then when we start making another commit, it just shifts the pointer to the child commit that we are making.

3. `HEAD` -> A pointer that exists in the git repository. It tells you that what branch you are working on, and what is the current commit is. Branch points to a commit and head points to a branch. Head will start moving when we actually make a new commit to a current branch. Initially master (a branch) is a pointer, pointing to a commit and Head points to a branch (master). Head always points to a current branch, so we can figure out on which branch we are currently working.

Note : Using branches we can work on a piece of code, without hampering another piece of code.

4. `git log --graph` -> to view current branch

5. `git branch` -> to view all the branches, and the star pointer indicates at which branch is head pointing to.

6. `git checkout <branch name>` -> to switch between branches

7. `git log --all --decorate --oneline --graph` -> to view entire branch structure
