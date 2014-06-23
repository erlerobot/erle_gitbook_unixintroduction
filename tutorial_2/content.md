
#### Displaying the contents of a file on the screen*

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
