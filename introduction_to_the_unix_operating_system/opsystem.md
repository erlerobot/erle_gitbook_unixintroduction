#### The UNIX operating system

The UNIX operating system is made up of three parts; the kernel, the shell and the programs.

#####The kernel

The kernel of UNIX is the hub of the operating system: it allocates time and memory to programs and handles the filestore and communications in response to system calls.

As an illustration of the way that the shell and the kernel work together, suppose a user types `rm myfile` (which has the effect of removing the file *myfile*). The shell searches the filestore for the file containing the program `rm`, and then requests the kernel, through system calls, to execute the program `rm` on *myfile*. When the process `rm myfile` has finished running, the shell then returns the UNIX prompt % to the user, indicating that it is waiting for further commands.

#####The shell

The shell acts as an interface between the user and the kernel. When a user logs in, the login program checks the username and password, and then starts another program called the shell. The shell is a command line interpreter (CLI). It interprets the commands the user types in and arranges for them to be carried out. The commands are themselves programs: when they terminate, the shell gives the user another prompt.

The adept user can customise his/her own shell, and users can use different shells on the same machine. For example we can use *tcsh shell* by default.

The tcsh shell has certain features to help the user inputting commands.

Filename Completion - By typing part of the name of a command, filename or directory and pressing the [Tab] key, the tcsh shell will complete the rest of the name automatically. If the shell finds more than one name beginning with those letters you have typed, it will beep, prompting you to type a few more letters before pressing the tab key again.

History - The shell keeps a list of the commands you have typed in. If you need to repeat a command, use the cursor keys to scroll up and down the list or type history for a list of previous commands

Another good choice is the *bash*.

A Shell is not just a shell. A Shell is chiefly an
interpreter of a powerful language
