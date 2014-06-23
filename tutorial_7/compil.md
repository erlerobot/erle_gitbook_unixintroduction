## Compiling UNIX software packages

We have many public domain and commercial software packages installed on our systems, which are available to all users. However, you can download and install other software packages in your computer.

There are a number of steps needed to install the software.

- Locate and download the source code (which is usually compressed)
- Unpack the source code
- Compile the code
- Install the resulting executable
- Set paths to the installation directory
- Of the above steps, probably the most difficult is the compilation stage.


#####Compiling Source Code

All high-level language code must be converted into a form the computer understands. For example, C language source code is converted into a lower-level language called assembly language. The assembly language code made by the previous stage is then converted into object code which are fragments of code which the computer understands directly. The final stage in compiling a program involves linking the object code to code libraries which contain certain built-in functions. This final stage produces an executable program.

To do all these steps by hand is complicated and beyond the capability of the ordinary user. A number of utilities and tools have been developed for programmers and end-users to simplify these steps.

##### make and the Makefile

The `make` command allows programmers to manage large programs or groups of programs. It aids in developing large programs by keeping track of which portions of the entire program have been changed, compiling only those parts of the program which have changed since the last compile.

The `make` program gets its set of compile rules from a text file called *Makefile* which resides in the same directory as the source files. It contains information on how to compile the software, e.g. the optimisation level, whether to include debugging info in the executable. It also contains information on where to install the finished compiled binaries (executables), manual pages, data files, dependent library files, configuration files, etc.

Some packages require you to edit the Makefile by hand to set the final installation directory and any other parameters. However, many packages are now being distributed with the GNU configure utility.

#####configure

As the number of UNIX variants increased, it became harder to write programs which could run on all variants. Developers frequently did not have access to every system, and the characteristics of some systems changed from version to version. The GNU configure and build system simplifies the building of programs distributed as source code. All programs are built using a simple, standardised, two step process. The program builder need not install any special tools in order to build the program.

The configure shell script attempts to guess correct values for various system-dependent variables used during compilation. It uses those values to create a Makefile in each directory of the package.

The simplest way to compile a package is:

1. `cd` to the directory containing the package's source code.
2. Type `./configure to configure the package for your system.
3. Type `make` to compile the package.
4. Optionally, type `make check` to run any self-tests that come with the package.
5. Type `make install` to install the programs and any data files and documentation.
6. Optionally, type `make clean to remove the program binaries and object files from the source code directory

The configure utility supports a wide variety of options. You can usually use the` --help `option to get a list of interesting options for a particular configure script.

The only generic options you are likely to use are the `--prefix `and `--exec-prefix` options. These options are used to specify the installation directories.

The directory named by the --prefix` option will hold machine independent files such as documentation, data and configuration files.

The directory named by the` --exec-prefix` option, (which is normally a subdirectory of the --prefix directory), will hold machine dependent files such as executables.
