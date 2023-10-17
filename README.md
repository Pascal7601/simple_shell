0x16. C - Simple Shell
This is the README file for the 0x16. C - Simple Shell project, created by Julien Barbier. This project is a simple UNIX command interpreter, often referred to as a shell. It was completed as a group project by Pascal Ndubi and Kelly NAMANO.

Project Description
The goal of this project is to create a basic command-line shell that can interpret and execute simple UNIX commands. The shell should be able to handle commands with arguments, manage the PATH, implement built-in commands (exit and env), handle separators (;), logical operators (&& and ||), aliases, variable replacement, and comments.

Concepts
For this project, you are expected to understand various concepts, including:

Basics of programming
Basics of C
Basics of thinking like an engineer
Group work
Learning how to learn
Project Details
Project Start Date: October 4, 2023, 6:00 AM
Project End Date: October 18, 2023, 6:00 AM
Checker Release Date: October 17, 2023, 3:07 AM
An auto-review will be launched at the deadline
Important Guidelines
Please keep the following guidelines in mind while working on this project:

Avoid copying code or looking at solutions from other sources. Originality and understanding are key.
Write code from scratch after gaining an understanding. Do not rewrite code from memory.
Do not share solutions or resources with others. Collaboration is encouraged, but copying is not.
Make use of AI tools like ChatGPT only at the appropriate stage and in line with the guidelines.
Focus on creating your own solutions rather than relying on external sources.
Learning Objectives
By the end of this project, you should be able to explain the following concepts:

The design and implementation of the original Unix operating system
The author of the first version of the UNIX shell
The inventor of the B programming language (the predecessor to C)
Who Ken Thompson is
How a shell works
What a pid and a ppid are
How to manipulate the environment of the current process
The difference between a function and a system call
How to create processes
The three prototypes of the main function
How the shell uses the PATH to find programs
How to execute another program with the execve system call
How to suspend the execution of a process until one of its children terminates
What EOF (end-of-file) means
Requirements
General
Allowed editors: vi, vim, emacs
All code files will be compiled on Ubuntu 20.04 LTS using GCC with the following flags: -Wall -Werror -Wextra -pedantic -std=gnu89
All code files should end with a new line
A README.md file at the root of the project folder is mandatory
The code should adhere to the Betty style
The shell should not have any memory leaks
Each code file should contain no more than 5 functions
All header files should be include guarded
Use system calls only when necessary
Write a README with the description of your project
Create an AUTHORS file at the root of your repository listing all contributors
GitHub
Only one project repository should exist per group, and both partners should be collaborators
Duplicating repository names in individual accounts can result in a 0% score
Output
The shell's output and error output should match those of /bin/sh
When printing an error, the program name (argv[0]) should be equivalent
List of Allowed Functions and System Calls
access
chdir
close
closedir
execve
exit
_exit
fflush
fork
free
getcwd
getline
getpid
isatty
kill
malloc
open
opendir
perror
read
readdir
signal
stat (__xstat)
lstat (__lxstat)
fstat (__fxstat)
strtok
wait
waitpid
wait3
wait4
write
Compilation
To compile your shell, use the following command:

shell
Copy code
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
Testing
Your shell should work in both interactive and non-interactive modes:

Interactive Mode:

shell
Copy code
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
Non-Interactive Mode:

shell
Copy code
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
Tasks
This project consists of several tasks, starting from creating a basic shell and gradually adding features such as handling arguments, implementing built-ins, managing environment variables, handling operators, and more.

Betty would be proud: Ensure your code adheres to the Betty style guide.

Simple shell 0.1: Create a basic shell that can execute simple UNIX commands and display a prompt.

Simple shell 0.2: Extend the shell to handle command lines with arguments.

Simple shell 0.3: Add the ability to handle the PATH and avoid unnecessary calls to fork when a command doesn't exist.

Simple shell 0.4: Implement the exit built-in command to exit the shell gracefully.

Simple shell 1.0: Implement the env built-in command to print the current environment variables.

Simple shell 0.1.1: Create your own getline function that reads input efficiently.

Simple shell 0.2.1: Implement string parsing without using the strtok function.

setenv, unsetenv: Add the setenv and unsetenv built-in commands for managing environment variables.

cd: Implement the cd built-in command to change the current directory.

;: Handle commands separated by semicolons.

&& and ||: Implement the logical operators && and || to control command execution based on success or failure.

alias: Create an alias built-in command for managing aliases.

Variables: Implement variable replacement, including special variables like $? and $$.

Comments: Handle comments in commands by ignoring lines that start with '#' (hash).

File as input: Allow the shell to accept a file as a command line argument, containing a list of commands to execute.

Authors
This project was created by Pascal Ndubi and Kelly NAMANO.
