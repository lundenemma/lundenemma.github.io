---
layout: default
---
## Command Line Tools for Linguists
The course is a basic intoroduction to the command line. Every courseweek consists of reading materials, tutorials with exercises, and quizzes.  
Many tasks practiced on the course are linguistically motivated. The course also has a final project, where the students use the skills learned on the course.  
 
### Week 1
Content:
* Introduction and installation of command line enviroments
* Basic commands

I learned to use very basic commands and the text editor nano.

Commands:

```wget [options] [url]```

Fetches a file from the internet

```mv [options] [source_file_name] [destination_file_name]```

Moves a file or a directory to another location, or  
renames a file or a directory

### Week 2
Content:
* How to manage directories
* Permissions in UNIX
* Working on a remote server

I learned how to manage file permissions that protect the user's privacy, how processes work and how to connect to the remote server puhti

Commands:

```ssh puhti.csc.fi```

Connects to the remote server puhti

### Week 3
Content:
* Using text processing tools
* Character encodings
* Structured text files

I learned how character encodings work and why converting between different encodings (ASCII, utf-8, Latin-1) is important. Also learned regural expressions for searching patterns. 

Commands:

```tr [options] 'SET1' 'SET2'```

Replaces characters, can be used to delete characters with option -d

```egrep [options] 'PATTERN' file```

Finds patterns in text files using regular expressions

### Week 4
<img src="assets/images/life_of_bee_trigram.png" alt="life of bee trigram" hspace="20" width="20%" height="30%" align="right"/>
Content:
* Continuation on using text processing tools
* Piping commands

I learned to pipe commands to do more complex operations easily, especially for text processing tasks like making frequency lists.

Commands:

```sed [options] [SCRIPT] [INPUTFILE]```

A versatile tool for editing files. Is used for finding and replacing strings, insertion, deletion, etc.

### Week 5
Content:
* Creating scripts 
* Configuration files

I learned to set up a configuration file for changing enviromental variables and using them I individualized my prompt.  
I also made scripts to make complex text processing task easier and faster. 

Commands:

```cat $1 |
dos2unix |
tr -s "[:space:]" "\n" |
tr -d "[:punct:]" |
sort |
uniq -c |
sort -nr > $2```

Script for creating frequency lists.  
Reads text file from standard input and through several text processing commands creates a numerically reversed list of word frequencies and directs the output to a file.

### Week 6
Content:
* Installing programs using package managers
* Running programs 

I learned to install Python packages and to use Python's standard package manager pip to handle the dependencies when installing programs.  
I also learned to use the make command for building projects.

Commands:

```sudo apt-get update```

This command updates the apt-get package manager, which is used in Linux systems. The sudo command grants the user the right to execute commands at the system level without switching users.

### Week 7
Content:
* Git, a version control system
* GitHub

I learned how to manage projects through version control, especially git. I also created an account (and started using it) in GitHub, a platfrom that provides git support. 

Commands:

```git branch```

Lists all the branches in a repository. The asterisk infront of the branch name denotes the current branch you are working in.

											
| Command 				| Description 			  		|
| ---					| ---						|
|					|						|
|```git add [file]``` 			| Adds a file to the staging area		|
| 					| 						|
|```git commit -m "[commit message]"``` | Commits changes				|
| 					| 						|
|```git push```				| Pushes changes to the the remote repository	|

With the commands shown in the table, the changes and modified versions of the files are committed and pushed to the remote repository.
