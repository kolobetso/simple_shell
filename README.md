## Simple Shell
> In this project, we coded from scratch a simple Unix shell. A shell is an interactive
> command-line interpreter. We created a shell that would utilize the command line
> interface (CLI). It allows users to type in a defined set of
> commands (e.g. "rm" to remove files, "cat" to combine word documents, etc) and have the
> operating system run the appropriate function. It is slightly different from a graphical user
> interface (GUI). For instance, instead of using a mouse to click to open folders and delete files, a user
> can type in a command (i.e. "ls" or "rm") and have the files be displayed or
> modified in a list on the command line. GUI and CLI both have the same purpose to interact
> with the operating system but their input methods are different and some developers
> prefer the CLI to interact with the shell because their typing is quicker than
> clicking and dragging. There are a few
> versions of Unix shells, from the very first (Ken Thompson's) shell that can
> be activated by typing ```sh``` in the terminal to today's most popular Bash
> (Bourne Again Shell). Later versions of the shell handle memory leaks better and

### Synopsis
> This repository holds all the code necessary for our custom simple shell to run.
> Our shell currently handles the executions of executables found in the
> environmental variable PATH, with or without their full paths. Sample commands
> that our shell supports include ```ls``` (```/bin/ls```), ```pwd```, ```echo```,
> ```which```, ```whereis```, etc. We've also created the following builtins.
### Builtins
check all builtin function
### Functions and system calls used
```read```, ```signal```, ```malloc```, ```free```, ```getcwd```, ```chdir```, ```access```, ```execve```, ```wait```, ```write```,  ```exit```and many other
### Description of what each file shows:
```
man_3_shell ------------------------ custom manpage for our simple shell
main.c ----------------------------- holds entrance into program
main.h ---------------------------- holds prototypes of functions spread across all files
```
Helper files
```
check all Helperfunctions
```
### Environment
* Language: C
* OS: Ubuntu 14.04 LTS
* Compiler: gcc 4.8.4
* Style guidelines: [Betty style](https://github.com/holbertonschool/Betty/wiki)
## How To Install, Compile, and Use
Install and Compile
```
(your_terminal)$ git clone https://github.com/Kolobetso/simple_shell.git
(your_terminal)$ cd simple_shell
(your_terminal)$ gcc -Wall -Werror -Wextra -pedantic -Wno-format *.c -o simple_shell
```
**Non-Interactive Mode**
```
echo "ls -l" | ./simple_shell
```
**Interactive Mode***
Activate the shell
```
(your_terminal)$ ./simple_shell
$
```
Sample Usage
```
$ ls -al
total 4
-rw-rw-r-- 1 vagrant vagrant   234 Mar 28 19:32 file1.c
-rw-rw-r-- 1 vagrant vagrant    69 Mar 28 19:32 file2.c
$ echo "This is a pretty cool!"
This is pretty cool!
$ man ./man_1_simple_shell (opens our manpage for more information)
```
Stop and return to your original shell
```
$ exit
(your_terminal)$
```
### To Do
* More functionality can still be added (e.g. handle aliases, pipelines, and redirections)
---
### Authors
Kolobetso Malepeng <jaquar93@gmail.com>
Banele Moeti <moetibanele5@gmail.com>
