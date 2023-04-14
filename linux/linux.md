Ubuntu - Based on linux, it is a linux distribution of debian type. Uses .deb packages.
For any linux command we can actually check the usage and different input flags it expects by running the command followed by --help.

Shell Scripting = It is a computer program designed to be run by a Unix shell, a command-line interpreter. The various dialects of shell scripts are considered to be scripting languages. Linux commands are part of shell scripts.

`REPL` - Read, evaluate, print, loop. - It is a sort of infinte loop - Reads command, evaluate expression, prints, and expects input again. - Every console is a REPL console only.

# Important commands for linux

1. `mkdir <>` -> creates a new folder.
2. `touch <>` -> creates a new blank file.
3. `cat <filename>` -> enables to read the contents of the file.
4. `pwd` -> current working directory.

5. `echo > text.txt "Hi"` -> // Writes content Hi in text.txt file, if we write echo again then
   it will delete previous content, and write new content in that file.

5a. `echo "Hello world"` -> This acts a print statement for terminal, similar to console.log in javascript

6. `ls` -> list of files in a particular folder.
   ls -l -> gives detailed list of the files and folders
   ls -a -> shows hidden folders
   ls -lh -> will also get the size of the file
   ls > text.txt -> instead of showing result on window, it will dump the result in text.txt file.

7. `rm <filename>` -> removes/deletes the file
   rmdir <folder name> -> deletes a folder only if folder is empty
   rm -r <folder name> -> deletes a folder along with its the files contained in it.
   rm -rf <folder name> -> forcefull delete of folder, along with its contents. Do not use it.

8. `cd <folder name>` -> change directory
   cd.. -> one step back
   cd ../.. -> two step back
   cd ~ -> moves back to home direclty from any folder
   cd / -> root directory, root does not have a parent. There is difference between root directory and home directory. Technically home directory is the sub-directory of root directory.

9. `~` -> this refers to the home directory
   cat ~/main.dart

10. `Relative path` -> It describes the location, of a file/folder with respect to current folder. Whereas in an absolute path we mention the location from home directory or root directory. When you give absolure path of a file or folder that means you will give the whole path of that file or folder, whereas in the relative path you do jumps with respect to the current folder.

11. `clear` -> clears the working space

12. `tail -n 3 <file name>` -> gives the last 3 lines of the file

13. `head -n 10 <file name>` -> gives the first 10 lines of the file

14. `|` -> pipe character, what ever is the result of first command is given as a input to second command. ex ls | grep -> result of ls is given as input to grep command.

15. `grep` -> used for string/substring matching/search.

16. `ps aux` -> gives the list of all the processes that are currently running.

17. `>` -> dumps the output of one command to a file. The entire previous date of other file gets replaced. ex pwd > test.txt

18. `>>` -> dumps the output of one command to a file. The entire previous date of other file gets appended not replaced. ex pwd > test.txt

19. `&&` -> combines multiple files, if first command is successfully executed only then second command gets executed. If first command fails, then it gives an error.

20. `cp <path of file or file name> <path of file or file name>` -> helps to copy data of one file to anther file.

21 `cp <path of file> <path of file>` -> move or cut-paste a file from one folder to another folder. This is also helpful in renaming a file.

22. `tar -cf archive.zip <file> <file>` -> combines both files, into one zip file.

23. `tar -zcf archive1.zip <file> <file>` -> compresses and combines both files into a single file.

24. `tar -xvzf archive1.zip` -> shows the content of zip file

25. `tar xf archieve1.zip -C <folder name>` -> to unzip the contents of a zip file to a particular folder.

26. `history` -> history of commands that you have run

27. `date` -> displays current date and time

28. `expr 2+2` -> displays 2+2 on screen

29.`wc <file name>` -> gives details of number of lines, words and no. of lines of a file.

30.`diff <filename> <filename>` -> content difference between two files.

# Vim

1. `vim new_file.text` -> create/open a file in vim

2. `esc :q` -> to close the file and exit vim.

3. `esc :wq` -> save the file and exit vim.

4. `esc :q!` -> forcefully close the file without saving it.

5. In normal node
   l: move the cursor right
   h: move the cursor left
   j: move the cursor down
   k: move cursor up
   dd: to delete the entire line
   gg: it will make the cursor, go to the first line
   G: it will make the cursor, go to the last line
   w: jump from one word to other word
   d2w: delete the word and jump to next
   yy: copy the whole line
   yw: copy one word.
   p: paste

6. `esc :s/foo/bar` -> to replace foo with bar
   esc :%s/foo/bar -> replace all occurances of foo with bar
