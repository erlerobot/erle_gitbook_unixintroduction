
#### 5.4 Listing suspended and background processes

When a process is running, backgrounded or suspended, it will be entered onto a list along with a job number. To examine this list, type

```
jobs
```

An example of a job list could be
```

[1] Suspended sleep 1000
[2] Running netscape
[3] Running matlab
```

To restart (foreground) a suspended processes, type

```
fg %jobnumber
```

For example, to restart sleep 1000, type

```
 fg %1
 ```

Typing `fg` with no job number foregrounds the last suspended process.


