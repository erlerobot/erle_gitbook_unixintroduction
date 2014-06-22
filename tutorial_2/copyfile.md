####2.2 Copying Files

`cp` *file1 file2* is the command which makes a copy of *file1* in the current working directory and calls it *file2*

What we are going to do now, is to take a file stored in an open access area of the file system, and use the cp command to copy it to your unixstuff directory.

First, cd to your unixstuff directory.
```
cd ~/unixstuff
```
Then at the UNIX prompt, type,
```
cp <path> .
```
You should write the path of the file you want to copy (e.g /Users/Marc/Downloads/science.txt). Don´t forget the dot at the end. REMEMBER, in Unix, dot means current directory.
The above command means copy the indicated file to the current directory, keeping the name the same.
