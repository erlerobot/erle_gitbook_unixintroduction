# Annex I: basic commands

| **Command** | **Meaning** |
|---------------|------------------|
| ls| list files in a directory|
| ls -a | list all files and directories|
| mkdir | make a directory|
| cd *directory* | change to the named directory|
| cd | change directory|
| cd ~ | change to the home directory|
| cd .. | change to th parent directory|
| pwd | display the path of the current directory|
| touch file| creates a file|
| echo ' test' | creates a text |
| cd *file1 file2*| copy file1 and call it file2|
| mv *file1 file2*| move or rename file1 to file2|
| rm file | remove a file|
| rmdir directory | remove a directory|
| cat file | display a file|
| less file | display a file a page at a time|
| head file | display the first few lines of a file|
| tail file| display the last few lines of a file|
|grep 'keyword' |file	search a file for keywords'|
|wc file|	count number of lines/words/characters in file|
| command > file |	redirect standard output to a file|
|command >> file|	append standard output to a file|
|command < file	|redirect standard input from a file|
|command1 *pipe* command2|	pipe the output of command1 to the input of command2|
|cat file1 file2 > file0|	concatenate file1 and file2 to file0|
|sort|	sort data|
|who|	list users currently logged in |
|*	|match any number of characters|
|?|	match one character|
|man command|	read the online manual page for a command|
|help command| short description of the use of the comman|
|whatis command|	brief description of a command|
|apropos keyword|	match commands with keyword in their man pages|
|ls -l |	list access rights for all files|
|chmod [options] |file	 change access rights for named file|
|command &|	run command in background|
|^C	|kill the job running in the foreground|
|^Z	|suspend the job running in the foreground|
|bg	|background the suspended job|
|jobs|	list current jobs|
|fg %1	|foreground job number 1|
|kill %1|	 kill job number 1|
|ps	|list current processes|
|kill 26152	|kill process number 26152(PID)|
|df |	space left on the system|
|du |kilobytes used by a directory|
|gzip|	reduces the size|
|gunzip|expands a file|
|zcat	|read gzipped files|
|file	|classifies the file according to its type|
|diff |compares the content of two files|
|find|	search through the directories|
|history	|keeps an ordered list of all the commands|
|^R|	 recursive search|
|ps	|list current processes|
|bc |calculator|
|make| compile the package|
|make check|  run any self-tests that come with the package|
|make install|  install the programs and any data files and documentation|
|tar -xvf|extract the contents of the tar file|
|./configure --prefix=*path*| run the configure utility setting the installation path to the selected one|
|./*programm*|run the programm(executable files)|
|printenv *pipe* less|show all values of environmment variables|
|set *pipe* less|show all values of shell variables|







