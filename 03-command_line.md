# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > 
My Cheat Sheet
`pwd`          print working directory  
`mkdir`        make a directory  
`rmdir`        remove a directory  
`touch fn`     create an empty file  
`rm fn`        remove a file  
`mv fn1 fn2`   rename from fn1 to fn2  
`ls -a`        list all files (including hidden)  
`cp dir/fn1 dir2`   copy file from dir to dir2 (directories)  
`history`      shows previous commands - can be executed with !num  
`head fn`      show first 10 lines of fn  
`grep "text" fn`    show lines in fn which contain "text"  
`!cmd`         execute last command that starts with cmd

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  
  
`ls`         list files in directory  
`ls -a`      list all files, including hidden  
`ls -l`      list files in long format (all the useful info on the files)  
`ls -lh`     lists files in long format with readable file size  
`ls -lah`    lists all files (including hidden) in long format with readable file size  
`ls -t`      lists files sorted by time and date  
`ls -Glp`    lists files in long format witha '\' after a directory showing different colors for file types  

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:  
  
`ls -d`      displays only directories  
`ls -1`      displays one file per line  
`ls -q`      displays non-printing characters  
`ls -R`      displays contents of directories as well  
`ls -r`      displays in reverse order  

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.  

'xargs' lets you pass the output of one command as the input of another 
ls foo* | xargs rm 

List all files that start with foo and remove them.   
This is quite simple as you could do rm foo* directly but this is the idea of xargs. 
