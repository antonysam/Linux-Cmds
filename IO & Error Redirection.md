Std Input Device - Keyboard/CommandLine

Std Output Device - Terminal

Std Error Device - Terminal

# Redirection

Usually all the error and output messages will be displayed in the terminal, and can also redirect to an external file

Types

| S.No| Redirection Type | Symbol| Number |
|-----|------------------|--------|-------|
| 1) | Output Redirection |  > >> | 1
| 2) | Error Redirection   | > >> | 2
| 3) |Input Redirection    | < | 0

---------------
# Output Redirection

# Cmd

e.g

_Displays the result only with in the terminal_
```
cat 
"press enter key"
<"User defined value">
```
_Displays the result in the file_
```
cat 1> <"filename"> or cat > <"filename">
```
_Append data in the existing file_
```
cat 1>> <"filename"> or cat > <"filename">
```
--------------
# Error Redirection

Note: 2 is mandatory for Error redirection or else it will consider as output redirection

# Cmd

e.g

_Displays the error in the file_
```
cal 14 2021 2> output.txt
```
_Append error in the existing file_
```
cal 14 2021 2>> output.txt
```
# Can more than one redirections in a same cmd
```
cal 14 2021 > output_redirection.txt 2> error_redirection.txt
```
---------------
# Input redirection  

_Displays the content in the file_

# Cmd
```
cat <inputredirectionfilename 
```
# Can more than one redirections in a same cmd

# Cmd
```
cat <inputredirectionfilename >outputredirectionfilename
```
------------
# Terminal redirection

Note: In Linux/unix everything is considered as file
      
_Displays the terminal location_

# Cmd
```
tty
```
_Display output data in another terminal in the same machine_

# Cmd
```
cal 1 2021 ><"terminal2 path">
```


