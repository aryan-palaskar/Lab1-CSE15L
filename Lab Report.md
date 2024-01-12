# Lab Report 1

## Command `cd`

**Markdown code showing the command with *no* argument and its output**
```
[user@sahara ~]$ pwd
/home
[user@sahara ~]$ cd
[user@sahara ~]$ pwd
/home
```
* The working directory was /home when the command was ran with no arguments.
* When the command was ran with no arguments it remained in the same directory because we didn't give it any path to change to. 
* The output wasn't an error because the default action of the command cd when no argument is given is to return to the /home directory.

**Markdown code showing the command with path to a *directory* as argument and its output**
```
[user@sahara ~]$ pwd
/home
[user@sahara ~]$ cd lecture1/
[user@sahara ~/lecture1]$ pwd
/home/lecture1
[user@sahara ~/lecture1]$ 
```
* The working directory was /home when the command was ran with path to directory as argument.
* The working directory changed  to /lecture1 after running the command with a path to the directory as argument because thats the type of argument `cd` command is seeking, its purpose is to change directory. 
* The output wasn't an error because we gave the `cd` a path to a directory which it was askiing. 

**Markdown code showing the command with path to a *file* as argument and its output**

```
[user@sahara ~]$ pwd
/home
[user@sahara ~]$ cd Hello.txt
bash: cd: Hello.txt: Not a directory
[user@sahara ~]$ 
```

* The working directory was /home when the command was ran with path to a file as argument.
* There was an error because the argument that we gave was a path to a directory we need to change to. 
* The output was indeed an error because the `cd` command is meant to run on path to files but directories. 

## Command `ls` 

**Markdown code showing the command with *no* argument and its output**
```
[user@sahara ~]$ pwd
/home
[user@sahara ~]$ ls
Hello.txt  lecture1
[user@sahara ~]$ 
```

* The working directory was /home when the command was ran with no argument. 
* I got that output from the command with no arguments because since /home is the current working directory, the command will just return all the files and directories in the current directory. 
* The output wasn't an error because the `ls` command when not provided a path would just return the contents of the current working directory. 

**Markdown code showing the command with *directory* argument and its output**

```
[user@sahara ~]$ pwd
/home
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
[user@sahara ~]$ 
```

* The working directory was /home when the command was ran with directory argument.
* I got the output from the command because we gave the `ls` command a path to a directory from which it should list all the files and folders. 
* The output didn't return an error because in the working directory /home we have a folder *lecture1* whose path the ls command can access and display its contents. 

**Markdown code showing the command with *file* argument and its output**

``` 
[user@sahara ~]$ pwd
/home
[user@sahara ~]$ ls Hello.txt
Hello.txt
```

* The working directory was /home when the command was ran with file argument.
* I got the output from the command because since the argument isn't a directory whose content can be shown, the `ls` command just lists the name of the file as is. 
* I didn't get an error because it just ran the path to file and listed the name of the file. 
