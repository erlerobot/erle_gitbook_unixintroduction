# Tutorial 2
---
For the next explanations and exercises, we will assume that science.txt is a txt file with the following text on it:
>The Electronic Telegraph  Thursday 28 September 1995  Science
This summer the Royal Observatory at Herstmonceux
found new life as a science centre. Andro Linklater
celebrates a partial victory for the heritage

>THE SIGHT of a child's top spinning unsupported in mid-air should have been
surprising. Rotating there in space, it not only defied the rules of gravity,
it defied common sense, and at least three Fellows of the Royal Society gazed
at it in something close to wonder.

>But this was Fabricators' Week at the Herstmonceux Science Centre, with
exhibitors from science centres all over Europe arriving to demonstrate
prototypes of experiments they hoped to produce as hands-on displays - a tube
of rocket-propelled rubber balls, a solar-powered toy car, a model of planetary
movement. They had a much tougher audience in mind. Would it astonish a child?

Please ensure you create and save this file in a known place.

####2.1 Creating files (required for next steps)

If you want to create a file you should use the command `touch`. First go to the directory where you are working using`cd`. Then create the file by typing:
```
touch science.txt
```
Now that the file is created you can write on it by using the command `echo`. First let's see what does this command.Type:
```
echo 'Hello'
```
You can read on your shell screen the text you have written between the '', *Hello* in this case.

If you type
```
echo 'Hello' > science.txt
```
You will have written the text onto the file.
Note: the > is a redirection character, we will matter about the this characters in the *tutorial 3*.

*working with erlerobot:*

![img_1](img2/erle_1.jpg)

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



####2.3 Moving files

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


####2.4 Removing files and directories

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

####2.5 Displaying the contents of a file on the screen*

#####clear (clear screen)

Before you start the next section, you may like to clear the terminal window of the previous commands so the output of the following commands can be clearly understood.

At the prompt, type

```
clear
```

This will clear all text and leave you with the % prompt at the top of the window.



#####cat (concatenate)

The command `cat` can be used to display the contents of a file on the screen. Type:

```
cat science.txt
```

As you can see, the file is longer than than the size of the window, so it scrolls past making it unreadable.


#####less

The command `less` writes the contents of a file onto the screen a page at a time. Type

```
 less science.txt
 ```

Press the [space-bar] if you want to see another page, and type [q] if you want to quit reading. As you can see, less is used in preference to cat for long files.



#####head

The `head `command writes the first ten lines of a file to the screen.

First clear the screen then type

```
head science.txt
```

Then type

```
 head -5 science.txt
 ```

What difference did the -5 do to the head command?
*Only shows the first 5 lines*


#####tail

The `tail` command writes the last ten lines of a file to the screen.

Clear the screen and type

```
 tail science.txt
 ```

*Q. How can you view the last 15 lines of the file?*
```
tail -15 science.txt
```


####2.6 Searching the contents of a file

Simple searching using `less`

Using `less`, you can search though a text file for a keyword (pattern). For example, to search through science.txt for the word 'science', type

```
 less science.txt
 ```

then, still in less, type a forward slash [/] followed by the word to search

```
/science
```

As you can see, less finds and highlights the keyword. Type [n] to search for the next occurrence of the word.



#####grep (don't ask why it is called grep)

`grep` is one of many standard UNIX utilities. It searches files for specified words or patterns. First clear the screen, then type

```
 grep science science.txt
 ```

As you can see, `grep` has printed out each line containg the word science (without capital letters)

Try typing

```
 grep Science science.txt
 ```

The `grep` command is case sensitive; it distinguishes between Science and science.

To ignore upper/lower case distinctions, use the -i option, i.e. type

```
 grep -i science science.txt
 ```

To search for a phrase or pattern, you must enclose it in single quotes (the apostrophe symbol). For example to search for spinning top, type

``` grep -i 'spinning top' science.txt```

Some of the other options of grep are:

-v display those lines that do NOT match
-n precede each matching line with the line number
-c print only the total count of matched lines
Try some of them and see the different results. Don't forget, you can use more than one option at a time. For example, the number of lines without the words science or Science is

```
 grep -ivc science science.txt
 ```



#####wc (word count)

A handy little utility is the `wc `command, short for word count. To do a word count on science.txt, type

```
 wc -w science.txt
 ```

To find out how many lines the file has, type

```
 wc -l science.txt
 ```

To finish, let's see some example of the commands.

 *working with erlerobot:*

 ![img_2](img2/erel _2.jpg)





 ####Summary

| **Command** | **Meaning** |
|---------------|------------------|
| touch file| creates a file|
| echo ' test' | creates a text |
| cd *file1 file2*| copy file1 and call it file2|
| mv *file1 file2*| move or rename file1 to file2|
| rm file | remove a file|
| rmdir directory | remove a directory|
| cat file | display a file|
| less file | display a file a page at a time|
| head file | display the first few lines of a file|
| tail file| display the last few lines of a file|
|grep 'keyword' |file	search a file for keywords'|
|wc file|	count number of lines/words/characters in file|


