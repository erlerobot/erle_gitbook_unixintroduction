## Passing parameters to the shell


| **Parameter** | **Meaning** |
|---------------|---------------|
|$0|value of the executed command itself|
|$1 |value of the 1st parameter|
|$2,$3 ...|value of the 2nd, 3rd...parameter|
|$#|number of parameters|
|$*|value of all concatened parameters|

For understanding better the table above, let's do a simply exercise.
Create a file called *parameters*.And edit it(we recommend you using `vi parameters`) with the following content:
```
echo 'param. number=' $#
echo '$0=' $0
echo '$1=' $1
echo '$2=' $2
echo '$3=' $3
echo '$*=' $*
```
Now, change the permissions using
```
chmod +x parameters
```

And execute the script with different parameters:

```
./parameters (no parameters)
./parameters hello (one parameter)
./parameters pa1 pa2 pa3 (three parameters)
```
*working with erlerobot:*

![param](img10/parameters.jpg)


