
####3.3 Redirecting the Input

We use the < symbol to redirect the input of a command.

The command `sort` alphabetically or numerically sorts a list. Type

```
 sort
 ```

Then type in the names of some animals. Press [Return] after each one.
```
dog
cat
bird
ape
^D (control d to stop)
```

The output will be
```
ape
bird
cat
dog
````

Using < you can redirect the input to come from a file rather than the keyboard. For example, to sort the list of fruit, type

```
sort < biglist
```

and the sorted list will be output to the screen.

To output the sorted list to a file, type,

```
sort < biglist > slist
```

Use cat to read the contents of the file slist
