# Tutorial 4
---

####4.1 Wildcards

#####The * wildcard

The character * is called a wildcard, and will match against none or more character(s) in a file (or directory) name. For example, in your unixstuff directory, type

```
 ls list*
 ```

This will list all files in the current directory starting with list....

Try typing

```
 ls *list
 ```


This will list all files in the current directory ending with ....list

#####The ? wildcard

The character ? will match exactly one character.
So ?ouse will match files like house and mouse, but not grouse.
Try typing

```
 ls ?list
 ```



####4.2 Filename conventions

We should note here that a directory is merely a special type of file. So the rules and conventions for naming files apply also to directories.

In naming files, characters with special meanings such as / * & % , should be avoided. Also, avoid using spaces within names. The safest way to name a file is to use only alphanumeric characters, that is, letters and numbers, together with _ (underscore) and . (dot).

|**Good filenames**	|**Bad filenames**|
|-------------------|-----------------|
|project.txt|	project|
|my_big_program.c|	my big program.c|
|fred_dave.doc|	fred & dave.doc|

File names conventionally start with a lower-case letter, and may end with a dot followed by a group of letters indicating the contents of the file. For example, all files consisting of C code may be named with the ending .c, for example, prog1.c . Then in order to list all files containing C code in your home directory, you need only type ls *.c in that directory.

####4.3 Getting Help

#####On-line Manuals

There are on-line manuals which gives information about most commands. The manual pages tell you which options a particular command can take, and how each option modifies the behaviour of the command. Type man command to read the manual page for a particular command.

For example, to find out more about the wc (word count) command, type

```
 man wc
 ```

Alternatively

```
 whatis wc
 ```


gives a one-line description of the command, but omits any information about options etc.

For some commands you can simply type
```
help cd
````
this command display helpful information about builtin commands.

##### Apropos

When you are not sure of the exact name of a command,

```
apropos keyword
```

will give you the commands with keyword in their manual page header. For example, try typing

```
apropos copy
```

