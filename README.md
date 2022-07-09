# Shell_scripting
What is Shell Scripting
Text files containing commands to execute by a shell are called shell scripts. In this, long and repetitive series of commands are compiled into a single script that can be stored and executed at any time, thereby reducing programming efforts. In shell scripts, repetitive work is largely avoided. The most common reason for using shell scripting is to program operating systems of Windows, UNIX, Apple, etc. In addition, companies use this script to develop an operating system with their own features. In terms of system-level operations, it is considered to be the easiest programming language to use. A shell script is referred to as a batch file in DOS operating system, and EXEC in IBM's mainframe VM operating systems. Shell scripts can be used for the following applications: 
![image](https://user-images.githubusercontent.com/59536110/178111113-e82f1f12-8004-40fe-86fc-51f4bf15d502.png)
Automation of the code compiling process.
Run a program or create an environment for programming.
Complete batch processing and file manipulation.
Integrate existing programs.
Perform routine backups.
Keeping an eye on a system.
System administration's tasks
Creating, maintaining, and implementing system boot scripts
A sample shell script: 
echo "hello world" 

Run it as follows: 
$ bash hello.sh 
# prints 
hello world 
Shell Scripting Interview Questions for Freshers
1. What is Shell?
A Shell is basically a command-line interpreter between user and kernel or a complete environment specially designed to run commands, shell scripts, and programs. In this, whenever a user enters human-readable commands (input commands) through the keyboard, the shell communicates with the kernel to execute these commands, and display output in a shell script. Just as there are different flavors of operating systems, there are also different types of shells. Every shell has its own set of commands and functions. Shells issue the prompt, $, called a command prompt. You can type into the prompt while it is displayed.  

After you press enter, your input is read by the shell. Based on the first word of your input, it determines the command you want to run. The characters in a word are separated using spaces and tabs.  

Example: 

Here is an example of a date command that displays the current date and time:  

$date Tue Aug 10 06:03:35 MST 2021![image](https://user-images.githubusercontent.com/59536110/178111131-e961c7f5-1882-47cb-948c-df03eb9d4436.png)
. Why is a shell script needed?
Shell scripts can be written for a variety of reasons:

Keeping repetitive tasks to a minimum.
Can be used by system administrators for routine backups.
Monitoring the system.
Adding new functions to the shell.
Shell scripting allows you to create your own tools.
System admin can automate daily tasks.
3. Write some advantages of shell scripting.
Shell scripting offers the following benefits:

An interactive debugging tool, as well as a quick start.   
Programmers need not change their syntax since both command and syntax are identical to those entered directly into the command line.  
Shell scripts are easy to use and quicker to write.   
It helps automate administrative tasks, so it is time-saving.   
As shell scripts are written in an interpreted language, they can be run without any additional effort on almost any modern operating system, including UNIX, Linux, BSD, and Mac OS X.  
They can be utilized for bulk execution rather than single instructions.   
Using it, you can develop your own custom operating system with relevant features.  
Software applications can be developed according to their respective platforms with this tool.

4. Write some limitations of shell scripting.
Shell scripting has the following disadvantages:

Errors are frequent and costly, and a single error can alter the command.  
The execution speed is slow. 
Bugs or inadequacies in the language's syntax or implementation.  
Large, complex tasks aren't well suited to it.  
Contrary to other scripting languages, etc., it provides a minimal data structure.   
Every time a shell command is executed, a new process is launched.
5. Name the file in which shell programs are stored.
A file called sh stores shell programs. Sh files contain commands written in a scripting language that is run by Unix shells.

6. Name different types of shells available.
Shells are divided into two categories: 
Bourne shell: The $ character is the default prompt when using a Bourne-type shell.
C shell: The % character is the default prompt when using a C-type shell.
The Bourne-type is subdivided into the following categories:

Bourne Again shell (BASH): This is the most common shell available on all Linux and based systems. It is open-source and freeware. In addition, it is an SH-compatible shell, with improved programming and interactive features over SH. It also allows you to efficiently perform many tasks.
Korn shell (KSH): Korn is basically a Unix shell that was initially based on the Bash Shell Scripting. It's a high-level language that's quite advanced. It has associative arrays and handles the loop syntax better than Bash. It is basically an improved version of Bourne shell.
The C-type is subdivided into the following categories:   

C shell (CSH): C shell is almost like C itself since it uses the shell syntax of the C programming language. In most cases, a command is executed either interactively from a terminal keyboard or from a file.
TENEX/TOPS C shell (TCSH): TCSH does not have a specific full name. TCSH is considered as an enhanced version of the CSH as it includes some additional features over CSH like command-line editing and filename or command completion. As with the previous version, it supports C-style syntax also.
7. Write difference between Bourne Shell and C Shell.
Bourne Shell: It has compactness and speed that set it apart from other shells. But it lacks interactive features such as the ability to recall previous commands. Additionally, the Bourne shell does not support arithmetic and logical expressions.
C Shell: It is a UNIX enhancement that incorporates interactive features like aliases and history of commands. Besides its built-in arithmetic and expression syntax, it also includes convenient programming features.
Difference between Bourne shell and C shell   

The C shell allows you to alias commands easily, whereas Bourne Shell does not allow this.
In the C shell, long commands can be used repeatedly, but not in Bourne.
Bourne does not have access to the command history, but the C shell does.
In the case of C, there is no need to repeatedly type the command.
8. What do you mean by Shell variable?
Shell variables are integral parts of all Shell programs and scripts. In general, we know that variables usually store data either in the form of characters or numbers. Shell also stores and manipulates information using variables in its programs. Generally, shell variables are stored as strings. Variables in the shell provide the information needed for scripts/commands to execute. In the following example, a shell variable is created and then printed: 

variable ="Hello" 
echo $variable 

9. What are different types of variables mostly used in shell scripting?
Shell scripts usually have two types of variables:  

System-defined variables: Also called environment variables, these are special built-in variables in the Linux kernel for each shell. They are normally defined in capital letters by the OS (Linux) and are standard variables.
Example:  
SHELL  
It is a Unix Defined or System Variable, which specifies the default working shell. 
User-defined variables: These variables are created and defined by users in order to store, access, read, and manipulate data. In general, they are defined in lowercase letters. The Echo command allows you to view them.
Example:    
$ a=10 
In this case, the user has defined the variable ‘a’ and assigned it the value 10.
10. Explain the term positional parameters.
In a shell program, positional parameters specify arguments that are used to launch the current process. A special set of variables is usually maintained by the shell for storing positional parameter values. Bash is an example of a shell that uses positional parameters. The bash shell can be used on Linux, BSD, macOS X, and Windows 10.

For example: 

mycommand one five "six four”   

In this case, the command name is mycommand, and there are four parameters in the command line: one, five, and "six four”.   

Note: A space delimits each positional parameter and each thing after spaces are interpreted by the shell as individual parameters. Therefore, the parameter itself should be enclosed in quotation marks if it contains a space, as in "six four".

11. What are control instructions?
Control instructions specify how the different instructions will be executed in the script. They are primarily used to determine the control flow in Shell programs. The execution of a shell script proceeds in succession without these instructions. In shell programs, control instructions govern how execution flows.

12. How many types of control instructions are available in a shell?
Shells provide four types of control instructions as given below:  

Sequence Control Instruction: This assures that a program's command runs in the sequence they are listed. As soon as the first command in the sequence has been completed, the second command follows, and so on.
Decision Control Instruction: It is also known as Selection Control Instruction. This instructs the computer which instruction it should execute next. In this, checking a condition is the basis for deciding which section to execute. If a given condition is True, a statement or set of statements will be executed; otherwise, they will be ignored.
Loop Control Instruction: It is also known as Repetition Instruction. This instruction allows a computer to continuously run a particular sequence of code. In a loop structure, the statements can be repeated until a condition is True or False, a particular number of times, or once for each element within the collection
Case-Control Instruction: This is used for selecting among several choices. Typically, they are used to execute only a particular block of statements within a series of statements.
13. Explain ways to create shortcuts in Linux.
Links present in Linux OS can be used to create shortcuts as given below: 

Hard Link: Hard links are mirror images of the originally linked files and are linked with an inode number. A hard-linked file remains even after the original file is deleted. Since hard links point to inodes, they cannot be implemented on directories. Hard links are created by the following command:
$ ln  [original filename] [link name]
![image](https://user-images.githubusercontent.com/59536110/178111176-e8f89bce-4ff3-4ab4-8ea6-4464dc8f7794.png)
Soft Link: Generally, soft links (also referred to as Symbolic links) are linked to the file name and can reside on the same as well as different file systems. When a soft link is created or deleted, it does not affect the original file, but when the original file is deleted, the soft link stops working. Typically, soft links are aliases (alternative paths) for the original file. Soft links are created by the following command:
$ ln  -s [original filename] [link name]
14. How to check whether a link is a hard one or a soft link?
We can use -h and -L operators of the test command to check whether a link is hard or soft (symbolic link).

-h file      //true if the file is a symbolic link
-L file      //true if the file is a symbolic link
One can also use:

readlink FILE; echo $?       // This returns 1 if it's a hard link and 0 if it's a symbolic link.

![image](https://user-images.githubusercontent.com/59536110/178111192-2cf93ae4-5499-4ce4-8462-3544e4534c69.png)

