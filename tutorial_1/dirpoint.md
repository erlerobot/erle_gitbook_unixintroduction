##The directories . and ..

Still in the unixstuff directory, type

```
ls -a
```

As you can see, in the unixstuff directory (and in all other directories), there are two special directories called (.) and (..)

#####The current directory (.)

In UNIX, (.) means the current directory, so typing

```
cd .
```
means stay where you are (the unixstuff directory).

*Notice that there is a space between cd and the dot.*

This may not seem very useful at first, but using (.) as the name of the current directory will save a lot of typing, as we shall see later in the tutorial.

#####The parent directory (..)

(..) means the parent of the current directory, so typing

```
cd ..
```

will take you one directory up the hierarchy (back to your home directory). Try it now.

Note: typing cd with no argument always returns you to your home directory. This is very useful if you are lost in the file system.
