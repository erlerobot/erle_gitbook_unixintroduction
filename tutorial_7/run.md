
####7.6 Running the software

You are now ready to run the software (assuming everything worked).

```
cd ~/units174
```

If you list the contents of the units directory, you will see a number of subdirectories.

- bin:	The binary executables
- info:	GNU info formatted documentation
man	Man pages
- share:	Shared data files

To run the program, change to the bin directory and type

```
cd bin
./units
```

As an example, convert 6 feet to metres.
```
You have: 6 feet
You want: metres

* 1.8288
```

If you get the answer 1.8288, congratulations, it worked.

To stop the programm you can simply type `^C`

To view what units it can convert between, view the data file in the share directory (the list is quite comprehensive).

To read the full documentation, change into the info directory and type

```
info --file=units.info
```
