####1.6 More about home directories and pathnames

Understanding pathnames

First type `cd` to get back to your home-directory, then type

```
ls unixstuff
```

to list the conents of your unixstuff directory.

Now type

```
ls backups
```

You will get a message like this -

backups: No such file or directory

The reason is, backups is not in your current working directory. To use a command on a file (or directory) not in the current working directory (the directory you are currently in), you must either `cd` to the correct directory, or specify its full pathname. To list the contents of your backups directory, you must type

```
ls unixstuff/backups
```



#####~ (your home directory)

Home directories can also be referred to by the tilde `~ `character. It can be used to specify paths starting at your home directory. So typing

```
ls ~/unixstuff
```

will list the contents of your unixstuff directory, no matter where you currently are in the file system.

What do you think

`ls ~`

would list?  *List the files in your home directory*
