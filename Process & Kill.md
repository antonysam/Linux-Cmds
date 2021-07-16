# Process

A instances of a running program

When we run a shell script or shell cmd a process will be created

# Types of process
```
1. foreground 
    e.g
     pwd
2. background
    e.g
     pwd & 
```
e.g 
_Displays the process id_

```
pwd &
```

# ps

_Usage_

_Displays the current running process_

# Cmd
```
ps
```
_Displays the running process with the user details_

# Cmd
```
ps -f
```
_Displays the all running process including internal process_

# Cmd
```
ps -e
```
Can also use -fe in a single cmd

# Cmd
```
ps -fe
```
_Displays the parent process along with the child process_

# Cmd
```
ps -H
```

-----------
_Creation of shell script file_

# Cmd
```
cat > <"filename">.sh
```
---------------

_Execute the shell script file_

# Note : press `ctrl+c` to forcefully exit the shell script execution

# Cmd
```
sh <"Shellscript-filename"> 
```
------------
# kill

_Stops the currently running process_

_kill the process_

# Cmd
```
kill <"pid">
```
_kill forcefully multiple process_

# Cmd
```
kill -9 <"pid"><"pid">
```




