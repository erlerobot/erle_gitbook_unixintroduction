
## Removing files and directories

`rm` (remove), `rmdir` (remove directory)

To delete (remove) a file, use the `rm` command. As an example, we are going to create a copy of the science.txt file then delete it.

Inside your unixstuff directory, type
```
cp science.txt tempfile.txt
ls
rm tempfile.txt
ls
```

You can use the `rmdir command to remove a directory (make sure it is empty first). Try to remove the backups directory. You will not be able to since UNIX will not let you remove a non-empty directory.

As  **exercise** you can create a directory called tempstuff using `mkdir` , then remove it using the `rmdir `command.

Create a directory called tempstuff using mkdir , then remove it using the rmdir command.
