####8.5 Setting shell variables in the .cshrc file

For example, to change the number of shell commands saved in the history list, you need to set the shell variable history. It is set to 100 by default, but you can increase this if you wish.

```
 set history = 200
 ```

Check this has worked by typing

```
echo $history
```

However, this has only set the variable for the lifetime of the current shell. If you open a new xterm window, it will only have the default history value set. To PERMANENTLY set the value of history, you will need to add the set command to the *.cshrc* file.

First open the *.cshrc* file in a text editor. An easy, user-friendly editor to use is nedit.

```
nedit ~/.cshrc
```
Or if you don't have it installes you can use vi text editor.
```
vi  ~/.cshrc
```
Add the following line AFTER the list of other commands.
```
set history = 200

```
If you are using [vi](http://www.radford.edu/~mhtay/CPSC120/VIM_Editor_Commands.htm):
```
set history = 200
<ESC> (for going to the command mode)
:w (for saving)
:q (for exit the programm)
```

Save the file and force the shell to reread its *.cshrc* file buy using the shell source command.

```
source .cshrc
```

Check this has worked by typing

```
echo $history
```
