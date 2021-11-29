# Linux permission

![](<../../.gitbook/assets/Screenshot from 2021-11-29 10-17-31.png>)

first field is represent  for owner and second for group and third for other&#x20;

![](<../../.gitbook/assets/Screenshot from 2021-11-29 10-19-33.png>)

```
-rwxrwxrwx  1 hide hide  491 Jun 21 20:15  test9.txt
permission on file
drwxr-xr-x  2 hide hide 4.0K Oct  4 14:44  test9
permission on directory

-----------------symbolic method to assign permission-------------

-   :  no permission
r   :  file or directory is readable
w   :  file or directory is writable
x   :  file or directory is executable

--------------numeric method to assign permission-----------------

0   :  no permission
4   :  file or directory is readable
2   :  file or directory is writable
1   :  file or directory is executable

------------------------------------------------------------------
umask value

# umask                               - to view umask value
after masking we get the default value of file
[666 - 022 = 644]                     - 022 is umask value
after masking we get the default value of directory
[777 - 022 = 755]                     - 022 is umask value

------------------------------------------------------------------

# chown user file/directory       -   change ownership
# chown -R user /dir              -   recursive mode 
# chown usr:grp file/dir          -   change owner user and group
# chown -R usr:grp /dir           -   recurcive for group and user
# chgrp group file/dir            -   change group file or directory
# chgrp -R group /dir             -   change group recursive
 
------------------------------------------------------------------

symbolic method for change permission
# chmod u+rwx file/dir            - add permission for user
# chmod g+rwx file/dir            - add permission for group
# chmod o+rwx file/dir            - add permission for other
# chmod u-rwx file/dir            - user permission remove
# chmod g-rwx file/dir            - group permission remove
# chmod o-rwx file/dir            - other permission remove
# chmod u=rw,g=rw,o=r file/dir
# chmod ugo+rw file/dir
chmod a=rwx test                  - a for all user group other

 
numeric method for change permission


# chmod 777 file/dir
# chmod 755 file/dir
# chmod 744 file/dir
# chmod 700 file/dir
# chmod -R 777 /dir                - -R for recursive

special permission
suid, sgid, sticky bit# chmod u+S file                  - set suid permission on file
# chmod 4755 file
# chmod u-s file                  - remove suid permission

------------------------------------------------------------------
# chmod g+s file                  - set sgid permission
# chmod 2755 file                  
# chmod g-s file                  - remove sgid permission

------------------------------------------------------------------

# chmod o+t /dir                  - set stickybit permission 
# chmod 1777 /dir    
# chmod o-t /dir                  - remove sticky bit
```
