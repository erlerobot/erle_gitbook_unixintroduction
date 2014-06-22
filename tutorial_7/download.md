
####7.2 Downloading source code

For this example, we will download a piece of free software that converts between different units of measurements.

First create a download directory
```
 mkdir download
 ```
 [Download the software here](https://github.com/silvianunez/erle_gitbook_unixintroduction/tree/master/tutorial_7/prog) and save it to your new download directory.

Now move it to *Erle*.You need to follow the process specified in annex III: [A new Erle terminal](../annex_iii_a_new_erle_terminal/README.md)

```
cd download
scp units-1.74.tar.gz root@11.0.0.1:~/
```
If you now  go to erle and list the content of your Home directory, you will have the file *units-1.74.tar.gz* there:
```
root@erlerobot:~# ls
otro  units-1.74.tar.gz

```
