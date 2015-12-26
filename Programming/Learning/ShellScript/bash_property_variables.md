# Special Shell Variables
---


***Process information***

| Variable    | Description |                            
|-------------|-------------|
| $$          | Process ID of shell |
| $PPID       | Process ID of shell’s parent process. |
| $?          | Exit status of last command. |
| $_          | Name of last command. |
| $!          | Process ID of last process run in the background using ampersand (&) operator. This is commonly used in conjunction with the wait builtin. |
| $PATH       | A colon-delimited list of locations where trusted executables are installed. Any executable in one of these locations can be executed without specifying a complete path. |


***Field and record parsing***

| Variable    | Description |
|-------------|-------------|
| $IFS        | Input Field Separators |

***User information***

| Variable    | Description |
|-------------|-------------|
| $HOME       | The user’s home directory. |
| $UID        | The user’s ID. |
| $USER       | The user’s (short) login name. |

***Miscellaneous Variables***

Variable    | Description |
------------|-------------|
| $#          | Number of arguments passed to the shell.|
| $@          | Complete list of arguments passed to the shell, separated by spaces.|
| $*          | Complete list of arguments passed to the shell, separated by the first character of the IFS (input field separators) variable.|
| $-          | A list of all shell flags currently enabled.|
| $PWD        | The current working directory. Equivalent to executing the pwd command.|