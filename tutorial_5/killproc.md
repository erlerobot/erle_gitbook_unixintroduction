
## Killing a process

`kill` (terminate or signal a process)

It is sometimes necessary to kill a process (for example, when an executing program is in an infinite loop)

To kill a job running in the foreground, type ^C (control c). For example, run

```
sleep 100
^C
```

To kill a suspended or background process, type

```
 kill %jobnumber
 ```

For example, run

```
sleep 100 &
jobs
 ```

If it is job number [4], type

```
kill %4
```


To check whether this has worked, examine the job list again to see if the process has been removed.

####ps (process status)

Alternatively, processes can be killed by finding their process numbers (PIDs) and using kill PID_number

```
sleep 1000 &
ps
```
```

PID TT S TIME COMMAND
20077 pts/5 S 0:05 sleep 1000
21563 pts/5 T 0:00 netscape
21873 pts/5 S 0:25 nedit
````


To kill off the process sleep 1000, type

```
kill 20077
```

and then type ps again to see if it has been removed from the list.

If a process refuses to be killed, uses the -9 option, i.e. type

```
kill -9 20077
```

Note: It is not possible to kill off other users' processes.
