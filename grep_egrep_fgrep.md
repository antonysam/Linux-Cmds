# grep Command
1. Global Regular Expressions Pattern - grep

_Searches a file with the given pattern_

# Cmd
```
grep <"pattern"> <"filename">
```
e.g
```
grep "sam" studenname

can also use with piping

ls -l|grep 'sam' student
```
# grep cmd options

_-i_ -> returns the result without considering the case

# Cmd
```
grep  <"pattern"> <"filename"> -i
```
_-n_ -> displays line numbers along with matched pattern

# Cmd
```
grep <"pattern"> <"filename"> -n
```
_-c_ -> counts number of times a searching pattern exists

# Cmd
```
grep <"pattern"> <"filename"> -c
```
_-v_ -> `v` represents verbose which displays lines not matches with the pattern

# Cmd
```
grep <"pattern"> <"filename"> -v
```
_-l_ ->displays files matches the pattern

# Cmd
```
grep <"pattern"> <"filename"> -l
```
_Displays the file starts with the given first character_

`^` represents the first character

# Cmd
```
grep '^<"First characters">' <"filename">
```
_Displays the file ends with the gien last character_

`$` represents the last character

# Cmd
```
grep '<"last charaters">$' <"filename">
```
_Displays the files with data in the given range of characters_

# Cmd
```
grep '[<"range of characters">'] <"filename">
```
e.g

# Cmd
```
grep '[A-D]' student
grep '[WER]' student
```
_search for vowels in the file_
```
grep '[aeiou]' student
```
_search for lines other than vowels in the file_
```
grep '[^aeiou]' student
```
--------------
# egrep 
Extented grep

_Search for multiple patterns_

`-e` ->represents for multiple patterns

e.g
# Cmd
```
grep -e "sam" -e "dany" student
```
can also use `egrep` cmd

or

# Cmd
```
egrep "(pattern1|pattern2)" <"filename">
```
-----------
# fgrep

`-F` ->search with fixed strings

Note: can't able to provide pattern

e.g

# Cmd
```
grep -F "sam
>Dany
>Linux" student 
```
or

# Cmd
```
fgrep "sam
>dany" student
```





