# chmod

_usage_

1. Can provide the permissions for a file

# Note: 
ls -l

-rw-r--r-- `-r` represents the file

drwxr-xr-x `d` represents the directory

# Roles

|S.No| Roles | Symbol |
|---|---|---|
|1.| owners/users| u |
|2.| groups | g |
|3.| others | o |

# Permissions

|S.No| Permissions | Symbol | Numeric representation |
|---|---|---|---|
|1.| read | r | 4 |
|2.| write | w | 2 |
|3.| execute | x | 1 |

# Cmd
``` 
chmod <owner-permission><group-permissions><other-permission> <"filename">
```
e.g

# Note : 
   4 -> read permissions for owner
   3 -> write and execute for group
   7 -> read write and execute for other
   
# Cmd
```
chmod 437 sample
```
