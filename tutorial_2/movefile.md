

#### Moving files

`mv` (move)

*`mv `file1 file2* moves (or renames) file1 to file2

To move a file from one place to another, use the mv command. This has the effect of moving rather than copying the file, so you end up with only one file rather than two.

It can also be used to rename a file, by moving the file to the same directory, but giving it a different name.

We are now going to move the file science.txt to your backups directory (the directory inside unixstuff).

First, change directories to your unixstuff directory. Then, inside the unixstuff directory, type
```
 mv science.txt backups/.
 ```

Type `ls `and` ls backups` to see if it has worked.
