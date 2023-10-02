# studying_shellcommand
studying shell command!

## function keys
- '>' : redirects output using this function after a command to create and save the output in a file
- '>>' : appends output to an extising file(if it already extists), or create and write to a new file(if it doesn't exist).
- '<' : redirects input from a file.
- you can mix "<", ">" together in a single line!
- '|' : the output of previous command becomes input of next command
- '\' : ignore line change in command(you can also use enter key)

-------------------------

## shell commands
```sh
$ cat :  displays the contents of a text file.
$ echo print :  simply print out the next sentences.
$ echo * :  show user what files are in.
$ echo ~ :  show user where the file in.
$ chmod :  changes permissions.
$ sudo some_command :  command as a superuser.
$ sudo -i :  command as a superuser always.
$ nano :  write and run a shell script.
$ history :  see previous command history.
```

----------------

## ***permissions***
linux is a multi-user system.  
Files and directories have a permission assinged differently to owner/group/others.  

example:  
-rwx rwx rwx  (r: read w: write x: execute)  
-: indicates regular file  
d: indicates directory  

------------------------------

## change permissions  

changing permissions uses binary numbers to write easier.  
which is,  
rwx rwx rwx = 111 111 111  
rw- rw- rw- = 110 110 110  
rwx --- --- = 111 000 000  

and it can be simply expressed...  
rwx = 111 in binary = 7  
rw- = 110 in binary = 6  
r-x = 101 in binary = 5  
r-- = 100 in binary = 4  

    
And here is a simple examples
 - 777: rwxrwxrwx
 - 755: rwxr-xr-x
 - 700: rwx------
 - 666: rw-rw-rw-
 - 644: rw-r--r--
 - 600:rw-------

---------------------------------

## Superuser
A superuser has all system administation authority.  
Some commands need superuser's privilleges.  
Put "sudo" before the command if you are a superuser.    

***Warning!! "sudo -i" means you will command as a superuser always. so it can be dangerous sometimes!***

------------------
# ***thanks for enjoying my lecture note!***
