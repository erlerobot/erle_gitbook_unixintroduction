## Wildcards

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
