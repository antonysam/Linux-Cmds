# Piping

_Usage_

1)Can pass output of one command as input for next command 

2)Using piping can make multiple commands to work together

3) ` | ` represents the piping symbol

# Cmd

_Sending output of cmd1 as an input to the cmd2_ 
```
<cmd1> | <cmd2> | <cmdn>....
```
# Demerit

1) In the middle of piping if we use redirection then it breaks piping 

e.g

# Cmd
```
ls -l / sample >output.txt | wc
```
In the above cmd the 1st cmd will execute properly and because of output redirection 

there is no input to the 2nd cmd. So, the piping breaks
---------------------------

# tee

can use `tee` while using output redirection and piping in the same command

![tee_explanation](https://github.com/antonysam/Linux-Cmds/blob/master/images/tee.PNG)

# Cmd
```
ls -l /sample | tee output.txt | wc
```
`tee` cmd will forward the input to next cmd if next cmd is not provided it will displayed in the terminal

# xargs

can use `xargs` while we need to pass the arguments from the cmd1 to next cmd

e.g

deletefiles.txt contains the files to be deleted 

1. cat tests.txt will display the content in the terminal `xargs` will get the stream and pass it to rm

# Cmd
```
cat tests.txt | xargs rm
```

