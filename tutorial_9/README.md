# Tutorial 9
---

#### 9.1 What is *vi* ?

*vi* is a screen-oriented text editor originally created for the Unix  operating system.
*vi* was designed for editing standard format file and nowadays can be use in a wide variety of sistems and terminals. One of the strong points of *vi* is its adaptability.
For Linux, exits a improved text editor called *vim*. One of the advantages of *vim* is the ability to undo receding one by one the latest changes.*Vim* also allows highlighting the certain files  syntax such as  .shellscript, html, C language, and other
many languages. These and other details make it very suitable for programming.
*Erlerobot* uses vim. You can find out this by typing:
```
vi
```

*working with erlerobot:*

![Vim](img9/Vim.jpg)



####9.2 Essential commands

Below are some tables containing the more usual *vim* commands. If you have more interest in *vim* commands or you are looking for other different commands, [here ](http://www.cs.rit.edu/~cslab/vi.html) you can find a more complete documentation.

#####Command line

| **Command** | **Meaning** |
|---------------|---------------|
|vi | edit a new file |
|vi file| edit a existing file|

#####Command mode

You get to command mode from the *entry mode* ("writing mode") by typing *Esc*.

| **Command** | **Meaning** |
|---------------|---------------|
|h | previous character|
|j or *enter* | next line|
|k|previous line|
|l or *space* | next character|
|L| last line|
|H| first line|
|M| central line|
|i | text entry - inserting|
|R| text entry - replacing |
|u| undu last modification|
|^R| undu the las *u* command|
|/ |Search a characters string|
|dd| remove a line|
|yy| save lines in the buffer|
|p|copy a buffer line, after the actual one|
|^G| show the name of the file, the number of lines, and the actual line|
|.|repeat last command
|ZZ| end saving the changes|

####Ex mode

You get to ex mode from the command mode by typing *:*.

| **Command** | **Meaning** |
|---------------|---------------|
|:*num*| position the cursor in the line *num* |
|:w | save|
|:w! | save forcing|
|:x| leave saving if necessary |
|:q|leave if there is no modification|
|:q!|leave without saving|
|:wq| leave saving changes|
|:set nu | number the lines|
|:set showmode|show the mode|








