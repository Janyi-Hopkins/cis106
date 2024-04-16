---
name : Ja'nyi Hopkins Walker
semester : spring 24
assignment : notes 5
---

# Notes 5 


## cat

### Definition
The cat command is used for displaying the content of a file.
### Usage
`cat` + `option` + `file(s) to display`
### Examples
* display the content of a file located in the pwd
  * `cat todo.lst`
* display the content of a file with line numbers
  * `cat -n ~/Documents/todo.md`
* display the content of a file showing non-printing characters
  * `cat -v ~/Documents/todo.md`


## tac

### Definition
The tac command is used for displaying the content of a file in reverse order.
### Usage
`tac` + `option` + `file(s) to display`
### Examples
* display the content of a file located in the pwd
  * `tac todo.md`
* display the content of a file using absolute path
  * `tac ~/Documents/todo.md`


## head

### Definition
The head command displays the top N number of lines of a given file.
### Usage
`head` + `option` + `file(s)`
### Examples
* display the first 10 lines of a file
  * `head ~/Documents/Book/dracula.txt`
* display the first 5 lines of a file
  * `head -5 ~/Documents/Book/dracula.txt`
* display the first line of multiple files using wildcards
  * `head -n 1 *.csv *.py`


## tail

### Definition
The tail command displays the last N number of lines of a given file.
### Usage
`tail` + `option` + `file`
### Examples
* display the last 10 lines of a file
  * `tail ~/Documents/Book/dracula.txt`
* display the last 5 lines of a file
  * `tail -5 ~/Documents/Book/dracula.txt`
* display a given number of lines of the output of a given command
  * `ls -l ~/cis106/ | tail -n 2`


## cut

### Definition
The cut command is used to extract a specific section of each line of a file and display it to the screen.
### Usage
`cut` + `option` + `file(s)`
### Examples
* display a list of all the users in your system
  * `cut -d ':' -f1 /etc/passwd`
* display a list of all the users in your system with their login shell
  * `cut -d ':' -f1,7 /etc/passwd`
* cut a range of bytes per line
  * `cut -b 1-5 usernames.txt`


## sort

### Definition
The sort command is used for sorting files.
### Usage
`sort` + `option` + `file`
### Examples
* sort a file
  * `sort users.lst`
* sort by column number
  * `sort -k 2 users.txt`
* sort and remove duplicate entries
  * `sort -u users.lst`


## wc

### Definition
The wc command is used for printing the number of lines, characters, and bytes in a file.
### Usage
`wc` + `option` + `file(s)` 
### Examples
* display the number of characters in a file
  * `wc -m users.txt`
* display the number of lines in a file
  * `wc -l users.txt`
* display the number words in a file
  * `wc -w users.txt`


## diff

### Definition
The diff command compares files and displays the differences between them
### Usage
`diff` + `option` + `file1` + `file2`
### Examples
* display the difference between two files
  * `diff cars.csv cars-backup.csv`
* display the difference between two files in a column format
  * `diff -y cars.csv cars-backup.csv`


## grep

### Definition
The grep command is used to search text in a given file
### Usage
`grep` + `option` + `search criteria` + `file(s)`
### Examples
* search any line that contains the word "dracula" in the given file
  * `grep 'dracula' ~/Documents/dracula.txt`
* search any line that contains the word "dracula" regardless of the case
  * `grep -i 'dracula' ~/Documents/dracula.txt`
* search any line that contains the word "dracula" regardless of case and with number line
  * `grep -in 'dracula' ~/Documents/dracula.txt`