 fully functional Unix-like shell with the following features:
Key Features:

Built-in commands: cd, pwd, exit
External commands: Executes any system command (like ls, cat, echo, etc.)
I/O Redirection:

> - output redirection (overwrite)
< - input redirection
>> - append redirection


Process management: Uses fork() and execvp() to run commands
Current directory display: Shows the current working directory in the prompt

To compile and run:
bashgcc -o myshell custom_shell.c -Wall
./myshell
Example usage:
bash/home/user$ ls -la
/home/user$ cd Documents
/home/user/Documents$ pwd
/home/user/Documents$ echo "Hello World" > output.txt
/home/user/Documents$ cat < output.txt
/home/user/Documents$ ls >> files.txt
/home/user/Documents$ exit
