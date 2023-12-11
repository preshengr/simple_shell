## 0x16. C - Simple Shell ##

A collabrative task in liu of our learning with ALX.
This project was desgined to test our ability to work together, brainstorm and come up with solutions.
Specific guidelines and requirements were met to make this project a success..

## General ##
System calls were used when necessary
Each file did not have more than 5 functions
Allowed editors: vi, vim, emacs
All files ended with a new line
All files were compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
Memory leaks where checked and none was found.
Betty coding style was strictly the standard for writing this code.
All header files include guarded

## GitHub ##
One repository was created and the other collaborated on the repository.

## Output ##
Unless specified otherwise, the shell program must have the exact same output as /bin/sh, including error output. The only difference is that when printing an error, the name of the program must be equivalent to argv[0].

Example of error with /bin/sh:
```
$ echo "qwerty" | /bin/sh
/bin/sh: 1: qwerty: not found
$ echo "qwerty" | /bin/../bin/sh
/bin/../bin/sh: 1: qwerty: not found
```
Same error with your program hsh:
```
$ echo "qwerty" | ./hsh
./hsh: 1: qwerty: not found
$ echo "qwerty" | ./././hsh
./././hsh: 1: qwerty: not found
```
## Description ##

**hsh** is a simple UNIX command language interpreter that reads commands from either a file or standard input and executes them.

### How _hsh_ works ##
* Prints a prompt and waits for a command from the user
* Creates a child process in which the command is checked
* Checks for built-ins, aliases in the PATH, and local executable programs
* The child process is replaced by the command, which accepts arguments
* When the command is done, the program returns to the parent process and prints the prompt
* The program is ready to receive a new command
* To exit: press Ctrl-D or enter "exit" (with or without a status)
* Works also in non interactive mode

## Compilation ##

The shell program was compiled using the following command:
```
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
```
## Testing ##

The shell program should work in both interactive and non-interactive modes.

**Interactive Mode**
```
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```
**Non-Interactive Mode**
```
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```
## Checks ##
All checks is according to ALX checker standard.

## Authors ##
The authors to this project was:
**PRECIOUS OKWUKWE AMAECHI**
- GitHub: [@preshengr](https://github.com/preshengr)
- Twitter: [@preshengr](https://twitter.com/preshengr)
- LinkedIn: [preshengr](https://www.linkedin.com/in/preshengr/)

**MAHLET MARESHA GIRMA**
- GitHub: [username](profilelink)
- LinkedIn: [username](profilelink)
- Twitter: [username](profilelink)



S I M P L E S H E L L
Introduction 🚀
The simple shell project is a collaboration between Oscar De León and Juan Camilo Villa, Software Engineering students at Holberton School, with which we can emulate the operation of a shell, which contains some of its most basic characteristics, such as : Handle PATH, Handle command lines with arguments.

Table of Contents
Description
Requirements
Installation and Compilation
Example of Use
Authors
Description 📖
Holberton School Shell (hsh), is a simple program of the line commands. This simple shell recreates basic and some more complex functionalities to result in our own Shell. This shell si developed in the programming language c. This shell takes the keyboard commands and delivers them to the system to be executed. some built-in commands implement: exit, env, help, cd.

Requirements 📋
Simple_shell is designed to run in the Ubuntu 14.04 LTS linux environment and to be compiled using the GNU compiler collection v. gcc 4.8.4 with flags -Wall, -Werror, -Wextra, and -pedantic.

Installation and Compilation🔧
Do you need clone this repository:

	git clone https://github.com/jcamilovillah/simple_shell
and then you can compile with this command:

	gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
after compilation you can excecute with this command:

	./hsh
Example of Use 💻
Compile the program to create the hsh executable file (see instructions above).
run the executable as follows ./hsh
Enter basic commands like: ls, you can add flags along with ls command such as -l, -la(ls -l, ls -la)
press enter after entering the command
to end the execution of the simple_shell program press ctrl + d or write the word exit
Your shell should work like this in interactive mode:

$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
But also in non-interactive mode:

$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
Authors ✒️
The authors to this project was:
**PRECIOUS OKWUKWE AMAECHI**
- GitHub: [@preshengr](https://github.com/preshengr)
- Twitter: [@preshengr](https://twitter.com/preshengr)
- LinkedIn: [preshengr](https://www.linkedin.com/in/preshengr/)

**MAHLET MARESHA GIRMA**
- GitHub: [username](profilelink)
- LinkedIn: [username](profilelink)
- Twitter: [username](profilelink)
 