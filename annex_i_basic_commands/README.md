# Annex I: basic commands
---


| **Command** | **Meaning** |
|---------------|------------------|
|*	|match any number of characters|
|./configure --prefix=*path*| run the configure utility setting the installation path to the selected one|
|./*programm*|run the programm(executable files)|
|?|	match one character|
|^C	|kill the job running in the foreground|
|^R|	 recursive search|
|^Z	|suspend the job running in the foreground|
|apropos keyword|	match commands with keyword in their man pages|
|bc |calculator|
|bg	|background the suspended job|
| cat file | display a file|
|cat file1 file2 > file0|	concatenate file1 and file2 to file0|
| cd | change directory|
| cd .. | change to th parent directory|
| cd ~ | change to the home directory|
| cd *directory* | change to the named directory|
| cd *file1 file2*| copy file1 and call it file2|
|chmod [options] |file	 change access rights for named file|
|command &|	run command in background|
|command < file	|redirect standard input from a file|
| command > file |	redirect standard output to a file|
|command >> file|	append standard output to a file|
|command1 *pipe* command2|	pipe the output of command1 to the input of command2|
|df |	space left on the system|
|diff |compares the content of two files|
|du |kilobytes used by a directory|
| echo ' test' | creates a text |
|fg %1	|foreground job number 1|
|file	|classifies the file according to its type|
|find|	search through the directories|
|grep 'keyword' |file	search a file for keywords'|
|gunzip|expands a file|
|gzip|	reduces the size|
| head file | display the first few lines of a file|
|help command| short description of the use of the comman|
|history	|keeps an ordered list of all the commands|
|jobs|	list current jobs|
|kill %1|	 kill job number 1|
|kill 26152	|kill process number 26152(PID)|
| less file | display a file a page at a time|
| ls| list files in a directory|
| ls -a | list all files and directories|
|ls -l |	list access rights for all files|
|make| compile the package|
|make check|  run any self-tests that come with the package|
|make install|  install the programs and any data files and documentation|
|man command|	read the online manual page for a command|
| mkdir | make a directory|
| mv *file1 file2*| move or rename file1 to file2|
|printenv *pipe* less|show all values of environmment variables|
|ps	|list current processes|
| pwd | display the path of the current directory|
| rm file | remove a file|
| rmdir directory | remove a directory|
|set *pipe* less|show all values of shell variables|
|sort|	sort data|
| tail file| display the last few lines of a file|
|tar -xvf|extract the contents of the tar file|
| touch file| creates a file|
|wc file|	count number of lines/words/characters in file|
|whatis command|	brief description of a command|
|who|	list users currently logged in |
|zcat	|read gzipped files|



