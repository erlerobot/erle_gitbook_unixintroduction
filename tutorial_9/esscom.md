
####9.2 Essential commands

Below are three tables containing the more usual *vim* commands. If you have more interest in *vim* commands or you are looking for other different commands, [here ](http://www.cs.rit.edu/~cslab/vi.html) you can find a more complete documentation.

#####Command line

| **Command** | **Meaning** |
|---------------|---------------|
|vi | edit a new file |
|vi file| edit a existing file|
|vi -r file| Edit recovering the changes not saved|
|vi file1 file2 ...|edit various files successively|

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
|u| undo last modification|
|^R| undo the las *u* command|
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
|:e file| edit simultaneously another file|
|:e #|Come back to the previous file|


