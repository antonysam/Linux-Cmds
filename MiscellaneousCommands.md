# touch

_Usage_

1)Create a new empty file

# Cmd

_creating the new empty file_ 
```
touch <"filename.extension"> 
```
Note: "." represents the hidden file 

_creating the new empty hidden file_
```
touch <".filename.extension"> 
```
----------

# ls

_Usage_

1)Lists the file

# Cmd

_listing the file_ 
```
ls
``` 
Note: -l represents the long list

_Listing the detail information of each files and directories_
```
ls -l
```
Note: -a represents the hidden file(hidden files starts with ".")

_Listing the detail information of each hidden files and directories_
```
ls -a
```
Note:hidden files starts with "."

_Listing the detail information of each files, hidden files and directories_
```
ls -l -a
```
Note:-F represents the slash "/"

_Listing the file and representing directories with "/"_
```
ls -F
```
Note:-r represents the reverse order

_Listing the file and  directories in the reverse order_
```
ls -r
```
Note:-R represents the directories with the sub-directories

_Listing the directories and sub-directories_
```
ls -R
```
Note:-S represents the files and directories size

_Listing the files and directories according to the highest size order_
```
ls -lS
```
_Listing the files present in the directories_
```
ls -l <"directoryname">
```
# Wildcard characters or Special characters
```
? - Single characters
* - Multiple characters
[] - Range of characters
```
_Listing the files using the special characters_

Note:single character file matches with all extensions
```
ls ?.* 
```
Note:single character file matches with .txt or .doc extensions
```
ls ?."txt"  or ls ?."doc" 
```
Note:lists the file name starts with character "a" and  with .txt 
```
ls a*."txt" 
```
Note:lists the file name starts with character "a" and  with .txt 
```
ls [<"character-range">].<"extension">

e.g ls [a-z]*.* 
```
----------
# head

_Usage_

1)Displays the file's top 10 lines in default

_Advantage_

1)We can use cat cmd only for smaller files but it is not suitable to view the content of a larger files

# Cmd

_Displaying the top 10 lines of the file_ 
```
head <"filename.extension"> 
```
Note: "-n" represents the no.of lines to be displayed 

_Displaying the lines of the file based on the user defined value_
```
head -n <"no.of.lines to be displayed"> <"filename.extension"> 
or
head -<"no.of.lines to be displayed"> <"filename.extension"> 
```
----------
# tail

_Usage_

1)Displays the file's last 10 lines in default

_Advantage_

1)We can use cat cmd only for smaller files but it is not suitable to view the content of a larger files

# Cmd

_Displaying the top 10 lines of the file_ 
```
tail <"filename.extension"> 
```
Note: "-n" represents the no.of lines to be displayed 
_Displaying the lines of the file based on the user defined value_
```
tail -n <"no.of.lines to be displayed"> <"filename.extension"> 
or
tail -<"no.of.lines to be displayed"> <"filename.extension"> 
```
# Can use head and tail in a single command inorder to get the no of lines in the middle 

#Cmd
```
head -<no.of.lines to be displayed"> <"filename.extension"> | tail -<"no.of.lines to be displayed">
```
# Can use head and tail with ls command
```
ls -l | head -<"no.of.lines to be displayed">
```
```
ls -l | tail -<"no.of.lines to be displayed">
```
-------
# more

_Usage_

1)Displays the file's content page by page

# Cmd

_Displaying the top 10 lines of the file_ 
```
more <"filename.extension"> 
"press spacebar inorder to traverse to one page another"
```
---------
# less

_Usage_

1)Displays the file's content page by page

_Advantage_

1) Using less cmd we can able to traverse to back and front but uisng more cmd we can able to move in forward direction only

# Cmd

_Displaying the top 10 lines of the file_ 
```
less <"filename.extension"> 
"upper arrow key inorder to traverse to previous page"
"press spacebar inorder to traverse to one page another"
```
# Can use less and more with ls command
```
ls -l | more
```
```
ls -l | less
```
-------

# who

_Display no of users connected to the current linux machine_

# Cmd
```
who
```
----------
# whoami

_Display the username of the current Linux machine_

# Cmd
```
whoami
```
----------
# hostname

_Display the hostname of the current Linux machine_

# Cmd
```
hostname
```
_Display the IP of the current Linux machine_

# Cmd
```
hostname -i
```
-----------
# uptime

_Display the current time, machine started time, connected users, load time of the machine_

# Cmd
```
uptime
```
-----------

# Cal

_Displays the current month calender_

# Cmd
```
cal 
```

_Displays the userdefined months in the calender_

# Cmd
```
cal <"month number"> <"year">
```
_Displays the pervious, current, next months in the calender_

# Cmd
```
cal -<no. of. months or year to be displayed">
```
_Displays the current month calender_

# Cmd
```
cal -m<"month number">
```
----------------
# date

Note: date --help shows different formats available for the date

_Displays the current date_

# Cmd
```
date "+%D"
```

_Display the date, month, year_

Note: Y - diaplays <"YYYY"> 
      y - diplays <"yy">
      
# Cmd
```
date "+%Y" or date "+%y"
date "+%m"
date "+%d"

or

date "+%d-%m-%Y"
date "+d/%m/%Y"
```
_Display the day and month in the words_

Note: a - displays <"Sun">
      A - displays <"Sunday">
      b - displays <"Dec">
      B - displays <"December">

# Cmd
```
date "+%a" or date "+%A"
date "+%b" or date "+%B"
date "+%d" or date "+%D"
```
_Display the current hour, minute, second _

Note: H - displays hour
      M - displays month 
      S - displas second
    
# Cmd
```
date "+<"user defined string"> %D %H/%M/%S
```





