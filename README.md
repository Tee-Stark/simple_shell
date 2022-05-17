**SHELLter** in Place, or Ship$, is a simple command line interpreter written in C.

### Deployment

This program was built in fulfilmint of alx software engineering programme

### Compilation

Ship$ is compiled this way:
`-Wall -Werror -Wextra -pedantic *.c -o hsh`

### To run the shell

`./hsh`

ShiP$ can run in interactive or non-interactive mode.

#### Interactive Mode

In interactive mode, run the program and wait for the `ShiP$` prompt to appear. Type commands freely, exiting with the `exit` command.

#### Non-Interactive Mode

In non-interactive mode, echo your desired command and pipe it into the program like this:

`echo "ls" | ./hsh`

In non-interactive mode, the program exits after finishing your  command(s).

### Commands

Ship$ runs executable commands in the PATH, and handles the following built-ins:

-   `exit [status]`
-   `env`
-   `setenv`
-   `unsetenv`
-   `cd`

Ship$ is also built to handle:

-   logical `&&` & `||`
-   comments beginning with `#`
-   commands separator `;`
-   `Ctrl-D`

### Example - Interactive Mode
`Ship$ ls`
`a.out	       double_free.c	    isin_dir.c		setenv_list2.c	_strtok.c
AUTHORS        get_cmds.c	    man_1_simple_shell	setenv_list.c	whitcher.c
authors.sh     get_tokens_strtok.c  put_prompt.c	shell.h
cd.c	       helpers1.c	    README.md		shellimg.jpeg
cmd_handler.c  helpers2.c	    rem_comments.c	simple_shell.c`</br>
`Ship$`

`Ship$ pwd` 
`/home/vagrant/simple_shell`
`Ship$ cd ..`
`Ship$ pwd`
`/home/vagrant`
`Ship$ `

`Ship$ which ls`
`/bin/ls`
`Ship$ `

`Ship$ exit`
`vagrant@vagrant-ubuntu-trusty-64:~/simple_shell$ `

### Example - Non-Interactive Mode
`vagrant@vagrant-ubuntu-trusty-64:~/simple_shell$ echo "ls" | ./hsh`
`a.out	       double_free.c	    hsh			rem_comments.c	simple_shell.c
AUTHORS        get_cmds.c	    isin_dir.c		setenv_list2.c	_strtok.c
authors.sh     get_tokens_strtok.c  man_1_simple_shell	setenv_list.c	whitcher.c
cd.c	       helpers1.c	    put_prompt.c	shell.h
cmd_handler.c  helpers2.c	    README.md		shellimg.jpeg`
`vagrant@vagrant-ubuntu-trusty-64:~/simple_shell$`

### Release History

-   0.0.1 - First release - 17 Apr 2020</br>

### About

All files were created and compiled on `Ubuntu 14.04.4 LTS` using `GCC 4.8.4` with the following flags: `-Wall -Werror -Wextra -pedantic`

### Collaborators

-   Ridwan ODUNOLA [Github](https://github.com/eXochus)
-   Timilehin Omolana [Github](https://github.com/Tee-stark)
