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

# Getting Help, Man Pages (man, type, help, apropos) Lesson 2
- 'man' short for manual

- man ls
    - type h
- to get out, q

- ctrl + f ~ moves 1 window going toward the end
- ctrl + b ~ moves 1 window going to the start

- g ~ beginning
- G ~ end

- Find a match
- type /string_argument
    - ex /sort
        - n to go to the next
        - N to go back
    -search backwards
    - ?sort

- 2 types of shell commands
    - executable (have command pages)
        - type ''
    - shell command 
        - type ''
        - To learn more, you need to do help ''

    - can get help as well doing
        - 'command' --help

- ifconfig
    - sudo apt install net-tools
    - searching all man pages


# Masting the terminal

- Use the tab key for auto completion

# Mastering the terminal ~ keyboard shortcuts

- ctrl + l 
    - clears screen

- ctrl + d
    - closes the terminal
    - can type exit too

- ctrl + a
    - move to beginning of the line

- ctrl + e
    - move to the end of the line

- ctrl + u
    - deletes all characters before the cursor but cutting

- ctrl + c
    - interrupt process running in the terminal
    - download a big file, and you need to stop it

- ctrl + z
    - pauses what is running
    - to restart bg %1

# Mastering the Terminal: Bash History

- Bash shell starts in user's home directory
- Number of commands controlled by env var call HISTFILESIZE
    - run echo $HISTFILESIZE
    - 2000 commands into the history file
    - type 'history'
        - Will see all commands
    - 1 is oldest command
    - highest number is newestecho 
    - $echo $HISTSIZE
        - 1000 commands in history
        - File updated when user locked out

- !(command)
    - run the last command

- !(command):(1st letter)
    - will show what it did

- ctrl + p 
    - previous command

- ctrl + n
    - walk forward

- recall mode ctrl + r
    - ctrl + g ~ clear the search

- remove history of command history
    - history -c


- HW
- How do you leave no trace in your HIST

- prefix with a space before the command
    - " echo "hello world"

- append history -d $(history 1)
    - "echo "hello"; history -d $(history 1)

- By setting flags to enable and siable history
    - disable
        - set +o history
    - enable
        - set -o history