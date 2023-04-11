1. `tags` -> tag is also a pointer, it can point to a particular commit. We can store some metadata inside tags, like message, author name etc..

Note : When we make a new commit, the branch pointer moves to that particular commit. But, the tag pointer never moves. It always points to the same commit.

2. `git show <tag name> ` -> to view a particular tag, that is pointing to a parituclar commit.

3. `git show-ref --tags` -> shows all the tags

4. `git push --tags origin master` -> to push tags separately on git hub.
