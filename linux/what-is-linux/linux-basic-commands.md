# linux basic commands

first we open terminal and one by one perform every commands&#x20;

![](<../../.gitbook/assets/Screenshot from 2021-11-29 01-25-40.png>)

### ----------------files and nevigating commands-----------------

**1. list all files and folder using ls command**

```
ls            -   list all files on current location
ls -l         -   listing formate
ls -lah       -   list formate and hidden files ,human readable
man ls        -   manual page for ls
ls --help     -   for help
```

&#x20;**2. show present working directory**

```
pwd
```

**3. change directory command**

```
cd name                -   for entering name directory
cd ..                  -   go back to one directory
cd ../../              -   go back two directory
cd ~                   -   change to home directory
cd /                   -   go to root / directory
cd --help              -   help of cp command
man cd                 -   manual page
```

**4. create a directory command**

```
mkdir dirname                -    create mydir directory
mkdir dir1 dir2              -    create multiple directory
mkdir -p dir1/dir2           -    create sub directory
mkdir --help
```

**5. remove directory command**

```
rmdir dirname                  -   remove a directory
rmdir dir1 dir2                -   remove multiple directory
rmdir -p dir1/dir2             -   remove sub directory
rm -r dirname                  -   delete directory
rmdir --help
```

**6. remove files command**

```
rm file                         -    delete single file
rm file1 file2                  -    delete multiple file
rm -r dirname                   -    delete directory and files
rm -rf dirname                  -    delete forcefully and recursive
rm -rf /*                       -    remove all files on / "don't use "
rm --help
```

**7.move file and directory**

```
mv file1 file2                  -  rename a file
mv file /tmp                    -  move file to directory
mv file dir/file1               -  move file to dir as a file1\
mv --help
```

**8. files creating command**

```
touch file.txt                 -  create a file
touch file1 file2              -  create multiple file
cat > file                     -  create  a file with cat
echo > file                    -  create a file with echo
vi file                        -  create a file with vi
vim file                       -  create a file with vim
nano file                      -  create a file with nano
```

**9. cat text editor**

```
cat file                          -   show content of file
cat /etc/passwd                   -   open passed file
cat > file.txt                    -   create a file
cat >> file.txt                   -   rewrite files
cat file.txt file1.txt > new.txt  - combnined file
cat test.txt | more               -   use cat with more command
cat test.txt | less               -   cat with less command
cat -n test.txt                   -   display line number
```

**10. nano text editor**

```
nano                             -   start a nano text editor
nano filename                    -   open file
```

**11. vim text editor**&#x20;

```
vim                               -    openning vim text editor
Vim - Modes
             1. Command mode
             2. Insert mode
vim file.txt                      -    open file command mode default
i                                 -    press i for insert mode
ese key                           -    for changing mode
:w                                -    save the file
:wq                               -    save file and exit
:q!                               -    exit without saving
file edit on command mode 
Deleting characters in command mode
x                                 -    delete single characters
5x                                -    delete 5 characters

Deleting Words
dw                                -     delete a word
5dw                               -     delete 5 word
Deleting Lines
dd                                -     delete one line
5dd                               -     delete 5 line
Copy paste line
yy                                -      copy a line
p                                 -      past a line
```

**12.Pipes and Redirects**

```

example of running multiple command

# ifconfig; data; ls;   
# pwd; ifconfig; id; who; -a; date
# ifconfig && date && ls
# pwd && ifconfig && id && who -a && date

------------------------pipes-------------------------------------

# ls -la |less                      -        show content page wise
# ls -la | more                     -        show content page wise
# ifconfig |grep inet               -        using multiple command

------------------------Redirection-------------------------------

# ls -la > newfile.txt              -        redirect output of ls command
# ls -lh /etc/ > /tmp/list.txt
# ls -lh /root/ >> /tmp/list.txt
# sort < file-numbers.txt

# cat /etc/shadow /etc/os-release /etc/sudoers

run this command without root user and see 

$ cat /etc/shadow /etc/os-release /etc/sudoers > /tmp/output.txt
$ cat /etc/shadow /etc/os-release /etc/sudoers 1> /tmp/st_out.txt
$ cat /etc/shadow /etc/os-release /etc/sudoers 2> /tmp/error.txt
$ cat /etc/shadow /etc/os-release /etc/sudoers 1> /tmp/out_2.txt 2> /tmp/error_2.txt     
$ cat /etc/shadow /etc/os-release /etc/sudoers 1> /tmp/out_2.txt 2> /tmp/error_2.txt
$ cat /etc/shadow /etc/os-release /etc/sudoers > /tmp/error.txt 2>&1
$ cat /etc/shadow /etc/os-release /etc/sudoers &> /tmp/error2.txt
$ cat /etc/*
$ cat /etc/* 1> /dev/null
$ cat /etc/shadow /etc/passwd > 1.txt
$ cat /etc/shadow /etc/passwd 1> 2.txt
$ cat /etc/shadow /etc/passwd 1> 2.txt
$ cat /etc/shadow /etc/passwd 2> 3.txt
$ cat /etc/shadow /etc/passwd > 2.txt
$ cat /etc/shadow /etc/passwd &> 3.txt
$ cat /etc/shadow /etc/passwd 1> 3.txt 2>&1

```

**13. Linux enviorment variable**

```
# echo $PATH
# echo $USER
# echo $PWD
# echo $HOME
# var1="my demo var"
# echo $var1
# env
```
