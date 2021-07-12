# cmp

_Usage_

1)Compares two files

# Cmd

_Displays the different lines by comparing two files_ 
```
cmp <"filename1"> <"filename2">
```
----------
# diff

Note: < represents the file1
      > represents the file2
      c - change
      d - delete
      a - add
      
_Displays the mismatches in first file with second file_

# Cmd
```
diff <"filename1"> <filename2">
```
# comm

_Usage_

1) It displays 3 columns in the output
   
   1st column - unique lines of 1st file
   
   2nd column - unique lines of 2nd file
   
   3rd column - common lines inn 2 files
 
_Pre-requsite_

1) Sort the files need to be compared 

# Cmd
```
comm <"filename1"> <"filename2">
```

