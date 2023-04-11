Hi, this is a demo file. This is created just for the purpose of git tutorial.

Important git commands -->

Repository -> It means git projects

1. `git init` -> Powers your folder to be managed by git, and initialises a new empty
   repository. It also creates a .git folder that has all the relevant logic to manage
   versions of your project.

2. `git status` -> status of files/git in the folder.

3. `working area` -> There can be bunch of files that are not currently handled by git.It means that changes done or to be done in those files are not managed by git yet. A file which is in the working area is considered to be not in the staging area. When we do 'git status' and we see a bunch of untracked files, then these are actually called to be in the working area.

4. `staging area` -> What all files are going to be part of the next version that we will create. This staging area is the place where git knows what changes will be done from the last version to the next version.

5. `git add` <file name> -> add file/files to the staging area, moves file from working area to staging area.

6. `git rm --cached` <file name> -> to remove a file from the staging area. File is actually moved to
   working area from staging area.

7. `repository area` -> This area actually contains the details of all your previous registered versions. And the files in this area, git already manages them and knows their version history.

8. `commit` -> Commit is a particular version of the project. It captures a snapshot of the project's staged changes and creates a version out of it.

9. `git commit -m <message>` -> registers staging changes to a commit.

10. `git log` -> lists down all the commits of the repository. If you want to exit out of git prompt press 'q'.

11. `git restore <file name>` -> it removes all file changes from the staging area to be committed. This can be useful, if we did some dirty piece of code and now no more want it. Instead of deleting every change line by line, we can restore it or you can say restore last clean version of the file.

12. `git restore --staged <file name>` -> It removes file from file changes from staging area to the working area. This only works if changes are in your staging area.

13. When we do 'git add <filename>' then changes move from working area to the staging area.

14. Difference between git rm and git restore(git rm --cached <filename>)
    ans: if you want to move the whole file back to the untracked state, then we do git rm.
    Otherwise if we just want to changes to be moved in working area and staging area,
    then we do git restore.

15. `git diff <commit id 1> <commit id 2>` -> compares two commits, and gives the difference of all file changes, between two commits.

16. `git diff <filename>` -> we can track changes in the file

17. `git remote` -> Helps to connect two repositories, i.e connect local repository(git init creates local repository), to git hub repository, when we type this command it gives the names all the of the remote connections.

18. `git remote add` -> create a new remote repository connection.

19. `origin` -> it is just a name of the remote connection, we can write anything instead of origin

20. `git remote rm` -> To remove remote connection between two repositories.

21. Every Commit is a Version.

22. `git remote add <name of remote> <link of remote>` -> This command helps us to add a new link to the remote repo and give a name to it.

23. `git remote rm <name of remote>` -> This command deletes a remote connection.

24. `git remote rename <old name> <new name>` -> This command renames the remote connection.

25. Note : The name of the remote connection is always used to establish communication between the repositories.

26. `git add <file 1> <file 2> <file 3>` -> this command will add multiple file changes together in the staging area.

27. `git add .` -> this command will add all files from working repositories to staging area.

28. `git pull <remote name> <branch name>` -> downloads latest changes from the branch of the mentioned remote in your local repo.

29. `rm -rf <folder name>` -> to delete entire folder with its contents

## Recommended Practices

    - make changes
    - git add <file name>
    - git commit
    - git pull
    - git push
