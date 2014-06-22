
####5.2 Changing access rights

`chmod` (changing a file mode)

Only the owner of a file can use `chmod` to change the permissions of a file. The options of `chmod` are as follows

|**Symbol**|**Meaning**|
|----------|-----------|
|u |user|
|g|group|
|o|other|
|a|all|
|r|read|
|w|write (and delete)|
|x|execute (and access directory)|
|+|add permission|
|-|take away permission|

For example; to remove,read ,write and execute permissions on the file biglist for the group and others, type

```
chmod go-rwx biglist
```

This will leave the other permissions unaffected.

To give read and write permissions on the file biglist to all,

```
 chmod a+rw biglist
 ```
In case you have a shell script and you want to make it an executable file,the command you should use is (remmember to cd first):

```
chmod +x script
```
As **exercise** try changing access permissions on the file science.txt and on the directory backups (Use ls -l to check that the permissions have changed).

