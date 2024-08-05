# The Linux Terminal in Depth

## Terminal, Consoles, Shells and Commands - Lesson 1

- What is a Terminal
    - A Terminal emulator and is a crucial part of any linux system because it allows you to access the system through the shell
    - A shell is aprogram that takes commands from the user and gives them to the OS kernal to execute. Also called the command interpreter. The shell gets started when the user logs in or starts the terminal
    - Linux is a case-sensitive OS

    - Most used - gnome terminal

- Shortcut to open ctrl alt t
- widely used is Bash shell

- what is the console
    - Special terminal if no GUI is started
    - ctrl alt f1 - f8
    - terminal and console used interchangablely 

- Structure of a linux command
    - ping 
        - Used to test network connection
        - network connectivity to destination hostping

    - ping -c 1 8.8.8.8
        - ping is a commandname
        - -c a command
        - 1 - seperating the argument
        - 8.8.8.8 argument

    - ping -c 1 127.0.0.1
        - ping is the name of the command
        - c is one of the command options
        - 1 is the option value
        - 127.0.0.1 is the argument
        - additional whitespaces if perfectly find, can be huge or just the 1

        - ping 127.0.0.1 -c 1 
            - perfectly fine to do but not the standard
            - this will send only 1 ping packet


- some commands that reguire and argument and some that don't
- some will return an error ~ just using and working in linux will help you learn

- df
    - displays information about file system and disc space

- ls -l /etc/

- ls --all and ls -a
    - they're the same
- df
    - displays information about the file system and storage