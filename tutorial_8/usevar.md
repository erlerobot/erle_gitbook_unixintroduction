
####8.4 Using and setting variables

Each time you login to a UNIX host, the system looks in your home directory for initialisation files. Information in these files is used to set up your working environment. The C and TC shells uses two files called *.login* and *.cshrc* (note that both file names begin with a dot).

At login the C shell first reads *.cshrc* followed by *.login*

*.login* is to set conditions which will apply to the whole session and to perform actions that are relevant only at login.

*.cshrc* is used to set conditions and perform actions specific to the shell and to each invocation of it.

The guidelines are to set ENVIRONMENT variables in the *.login* file and SHELL variables in the *.cshrc* file.

WARNING: NEVER put commands that run graphical displays (e.g. a web browser) in your *.cshrc* or *.login* file.
