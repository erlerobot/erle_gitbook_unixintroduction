
####8.6 Setting the path

When you type a command, your path (or PATH) variable defines in which directories the shell will look to find the command you typed. If the system returns a message saying "command: Command not found", this indicates that either the command doesn't exist at all on the system or it is simply not in your path.

For example, to run units, you either need to directly specify the units path (~/units174/bin/units), or you need to have the directory ~/units174/bin in your path.

You can add it to the end of your existing path (the $path represents this) by issuing the command:

```
set path = ($path ~/units174/bin)
```

Test that this worked by trying to run units in any directory other that where units is actually located.

```
cd
units
```

To add this path PERMANENTLY, add the following line to your *.cshrc* AFTER the list of other commands.

```
set path = ($path ~/units174/bin)
```
