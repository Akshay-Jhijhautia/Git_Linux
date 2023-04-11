1. `tree .git` -> gives the structure of .git folder. this will help us see git folder in tree like structure

2. `echo 'Hello git' | git hash-object --stdin` -> This gives 40 digit hexa-decimal hash code, it is similar to 40 digit hash that we get when we a new file in git.

3. `echo 'Hello git' | git hash-object -w --stdin` -> this will write the 40 digit key in the .git folder

4. `git add <filename>` -> this adds the file in the .git folder. This file can be visualised by viewing structure of .git structure.

5. `git cat-file -p 5b916c915b5a2f39c3902152b114911b5f34aeb2` -> to view/print the file in the .git folder

6. `git cat-file -t 5b916c915b5a2f39c3902152b114911b5f34aeb2` -> it shows the type of file, whether it is a blob or a tree or a commit.

7. `commit` -> commit actually represents one particular version, it is basically a snapshot of our repository/code at some particular time. Commit also gets stored in .git folder, it is also stored in the form of key-value pair. Where key is the hash and the value is commit object.

8. `commit object` -> it is a separate object stored inside git. It contains details like author, reference to tree, how has commited the commit. Commit id is always different i.e commits are always unique. After the first commit, when we do commit, then commit object has an addtional property of parent hash commit. A commuit always points to the parent commit.

9. `git gc` -> garbage collection, it is similar to when we push code to repository. It dumps everything and creates a pack file of the hashes contained in the .git folder. This is done to optimise the functioning. Similarly when we push the code to the repository, all the hashes are combined into the pack file i.e commpressed version of everything, to achieve efficiency.

10. `git verify-pack -v .git/objects/pack/pack-09f20e283c540eb9ad215a4e6732e401b09af0a9.idx` -> this command gives the details of everything mentioned in the pack. Pack contains all the hash files i.e blob, tree, commits.

Note: Whatever changes happen by `git add` or `git commit`, these changes happens in the objects folder of the .git folder
