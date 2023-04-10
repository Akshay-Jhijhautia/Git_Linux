1. `tree .git` -> gives the structure of .git folder

2. `echo 'Hello git' | git hash-object --stdin` -> This gives 40 digit hexa-decimal hash code, it is similar to 40 digit hash that we get when we a new file in git.

3. `echo 'Hello git' | git hash-object -w --stdin` -> this will write the 40 digit key in the .git folder

4. `git add <filename>` -> this adds the file in the .git folder. This file can be visualised
   by viewing structure of .git structure.
