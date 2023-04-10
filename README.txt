Hi, this is a demo file. This is created just for the purpose of git tutorial

Important git commands

1. git init -> Powers your folder to be managed by git, and initialises a new empty 
repository. It also creates a .git folder that has all the relevant logic to manage 
versions of your project.

2. git status -> status of files/git in the folder.

3. 'working area' -> There can be bunch of files that are not currently handled by git.
It means that changes done or to be done in those files are not managed by git yet. A file
which is in the working area is considered to be not in the staging area. When we do 'git status' 
and we see a bunch of untracked files, then these are actually called to be in the working area.

4. 'staging area' -> What all files are going to be part of the next version that we will create.
This staging area is the place where git knows what changes will be done from the last version to
the next version.

5. git add <file name> -> add file/files to the staging area, moves file from working area to 
staging area.

6. git rm --cached <file name> -> to remove a file from the staging area. File is actually moved to
working area from staging area.

7. repository area -> This area actually contains the details of all your previous registered versions.
And the files in this area, git already manages them and knows their version history.

8. commit -> Commit is a particular version of the project. It captures a snapshot of the project's staged
changes and creates a version out of it.

9. git commit -> registers staging changes to a commit.

