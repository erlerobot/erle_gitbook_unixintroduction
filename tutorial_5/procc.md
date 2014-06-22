
####5.3 Processes and Jobs

A process is an executing program identified by a unique PID (process identifier). To see information about your processes, with their associated PID and status, type

```
ps
```


A process may be in the foreground, in the background, or be suspended. In general the shell does not return the UNIX prompt until the current process has finished executing.

Some processes take a long time to run and hold up the terminal. Backgrounding a long process has the effect that the UNIX prompt is returned immediately, and other tasks can be carried out while the original process continues executing.


*working with erlerobot:*

![process](img5/11_Fotor.jpg)


#####Running background processes

To background a process, type an & at the end of the command line. For example, the command sleep waits a given number of seconds before continuing. Type

```
 sleep 10
 ```

This will wait 10 seconds before returning the command prompt %. Until the command prompt is returned, you can do nothing except wait.

To run sleep in the background, type

```
sleep 10 &
```
```

[1] 6259
```

The & runs the job in the background and returns the prompt straight away, allowing you do run other programs while waiting for that one to finish.

The first line in the above example is typed in by the user; the next line, indicating job number and PID, is returned by the machine. The user is be notified of a job number (numbered from 1) enclosed in square brackets, together with a PID and is notified when a background process is finished. Backgrounding is useful for jobs which will take a long time to complete.

####Backgrounding a current foreground process

At the prompt, type

```
 sleep 1000
 ```

You can suspend the process running in the foreground by typing ^Z ( i.e.hold down the [Ctrl] key and type [z]). Then to put it in the background, type

```
bg
```

Note: do not background programs that require user interaction: e.g. vi (text editor)
