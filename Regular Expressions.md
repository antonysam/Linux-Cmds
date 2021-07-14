# Regular Expressions

1. Also known as regex

2. Pattern for a matching string
---------

_Usage_

1. Used with different cmds like ls, rm, grep, sed, rename e.t.c
-----------

# Cmd

_list files name with atleat 3 chars_ 

Note: `*` represents all files

      `?` represents single character
```
ls ???*
```
-----------
_list files name starts with 'c' & ends with 's'_ 

Note: `*` represents all files

```
ls c*s
```
------------
_list files name starts with 's' or 'r' aplhabet_ 

Note: `*` represents all files

```
ls [sr]*
```
-------------
_list files name that not starts with 's' or 'r' aplhabet_

Note: `!` represents not equal

```
ls [!sr]*
```
--------------

_list files name starts with lower case aplhabet_ 

Note: `-` represents the range

```
ls [a-z]*
or 
ls[[:lower:]]*
```
------------
_list files name starts with upper case aplhabet_
```
ls[A-Z]*
or
ls[[:upper:]]*
```
-------------
_list files name starts with digit_
```
ls[0-9]*
or
ls [[:digit:]]*
```
-----------
_list files name starts with 1st letter upper 2nd letter lower 3rd letter digit_
```
ls [A-Z][0-9][a-z]*
or
ls [[:upper:]][0-9][[:lower:]]*
```
--------
_list files name starts with special symbol_

Note: alnum file name can starts upper lower or digit, but we need special symbols so we can use `!`

```
[![:alnum:]]*
```
_list files name with different extensions_
```
ls{*.java, *.py}
```
----------
