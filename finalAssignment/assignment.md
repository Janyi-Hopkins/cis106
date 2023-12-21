---
name : Ja'nyi Hopkins Walker
course : cis106
semester : fall 23
---

# Final Assignment Submission 

## Question 1

### Awk
* Description
  * Awk is used to display and process text. Cna work with text file or standard output.
* Syntax/Formula
  * awk + options + {awk command} + file + files to save (optional)
* Examples
  * Print first column of every line of a file
      * awk '{print $1}' ~/Documents/Csv/cars.csv
  * Prints last field of a file
      * awk -F: '{print $NF}' /etc/passwd
  * Converts first field to upper/lower case
      * awk -F: '{print toupper($1)}' /etc/passwd

### Cat
* Description
  * Cat is used for displaying a files content.
* Syntax/Formula
  * cat + option + file(s) to display
* Examples
  * Display content of a file
      * cat todo.lst
  * Display content with line numbers
      * cat -n ~/Documents/todo.lst
  * Displays content of a file using absolute path
      * cat ~/Documents/todo.lst

### Cp
* Description
  * Cp is used to copy files from one place to another. Similar to mv command.
* Syntax/Formula
  * cp + files to copy + destination
* Examples
  * Copy directories with absolute path
      * cp -r ~/Downloads/Wallpapers ~/Pictures/
  * Copy multiple files in a single command
      * sudo cp -r script.sh program.ny home.html assets/ /var/www/html/
  * Copy content of a directory to another directory
      * cp Downloads/Wallpapers/* ~/Pictures/

### Cut
* Description
  * Cut is used to extract a specific section of a file and display it on screen.
* Syntax/Formula
  * cut + options + files
* Examples
  * Display list of all users in your system
      * cut -d ':' -f1 /etc/passwd
  * Display range of bytes per line
      * cut -b 1-5 usernames.txt
  * Display a file excluding the given field
      * cut -d ',' --complement -s -f3 users.txt

### Grep
* Description
  * Grep is used to search text in given files.
* Syntax/Formula
  * grep + option + search criteria + file(s)
* Examples
  * Search any line that contains the word dracula
      * grep 'dracula' ~/Documents/Dracula.txt
  * Search for all the lines that ends with the string "nologin"
      * grep -n 'nologin$' /etc/passwd
  * ^ symbol matches the empty string at the beginning of a line.
      * grep -ni '^dracula' ~/Documents/Books/dracula.txt

### Head
* Description
  * Head is used to display the top N number of lines of a given file.
* Syntax/Formula
  * head + option + file(s)
* Examples
  * Display first 10 lines
      * head ~/Documents/Book/dracula.txt
  * Display first 5 lines
      * head -5 ~/Documents/Books/dracula.txt
  * display first 20 lines
      * head -20 ~/Documents/Books/dracula.txt
  
### Ls
* Description
  * Ls is used to list content of a directory or file/directory.
* Syntax/Formula
  * ls + option + directory to list
* Examples
  * list all files including hidden files
      * ls -a
  * list all files inside a given directory
      * ls -a ~/Pictures
  * long list all the files inside a given directory recursively
      * ls -lR ~/Pictures

### Man
* Description
  * Man is used to display the user manual of any command that can run on the terminal.
* Syntax/Formula
  * man + command name 
* Examples
  * manual pages of printf command 
      * man printf
  * using manual to get the section where command ls is present by using f
      * man -f ls
  * using manual to search the command ls location in a file using w
      * man -w ls

### Mkdir
* Description
  * Mkdir is used to make/create single or multiple directories.
* Syntax/Formula
  * mkdir + name o directory
* Examples
  * make a directory in present working directory
      * mkdir wallpapers
  * create a directory with a space in the name
      * mkdir wallpapers/new\ cars or mkdir wallpapers/'cities usa'
  * create a directory with a parent directory at the same time
      * mkdir -p wallpapers_others/movies

### Mv
* Description
  * Mv is used to move and rename directories.
* Syntax/Formula
  * mv + source + destination
  * mv + file/directory to rename + new name
* Examples
  * move a file to a directory to another using relative path
      * mv Downloads/homework.pdf Documents/
  * move multiple directories/files to a different directory
      * mv games/ wallpapers/ rockmusic/ /media/student/flashdrive/
  * move and rename in one command
      * mv Downloads/cis106homework.docx Documents/new_cis106homework.docx

### Tac
* Description
  * Tac is used to display content of a file in reverse order.
* Syntax/Formula
  * tac + option + file(s) to display
* Examples
  * display content of file located in pwd
      * tac todo.md
  * display content of file using absolute path
      * tac ~/Documents/todo.md
  * display content of the /etc/passwd file
      * tac /etc/passwd

### Tail
* Description
  * Tail display the last N number of a given file.
* Syntax/Formula
  * tail + option + file
* Examples
  * display last 10 lines of a file
      * tail ~/Documents/Book/dracula.txt
  * display last 5 lines of a file
      * tail -5 ~/Documents/Book/dracula.txt
  * Display last user in file
      * tail -1 /etc/passwd

### Touch
* Description
  * Touch is used to create files
* Syntax/Formula
  * touch + file name
* Examples
  * create file called list
      * touch list
  * create file with space in its name
      * touch Downloads/games2.txt
  * create several files at once
      * touch list_of_cars.txt script.py names.csv

### Tr 
* Description 
  * Tr is used to translate and delete characters from standard output
* Syntax/Formula
  * standard output | tr + option + set + set
* Examples
  * translate one character to another
      * cat file.txt | tr '.' ','
  * translate space to tab
      * cat program.py | tr "[:space:]" '\t'
  * translate tab to space
      * cat cars.csv | tr -s "[:space:]" ' '

### Tree
* Description 
  * Tree is used to display the entire structure of a file system, directories and files.
* Syntax/Formula
  * tree + options + directory
* Examples
  * display all files including hidden files
      * tree -a
  * display directories only
      * tree -d
  * display directory structure
      * tree

## Question 2

*How to work with multiple terminals open?

* How to work with multiple terminals open?
  * You can with multiple directories open by opening multiple windows within tilix or the terminals.
* How to work with manual pages?
  * You would use the scroll wheel or arrows to navigate the the pages.
* How to parse (search) for specific words in the manual page?
  * You can search for specific words by doing / and then what you are looking for.
      * ex: /reverse you would see all the places the word reverse takes place
* How to redirect output (> and |)
  * You would use > to redirect output to a file and you would use | to redirect output to another command.
      * ex: name > file.txt
      * ex: page1 | page3
* How to append the output of a command to a file?
  * You would use the operator >>.
      * ex: name >> truth.py
* How to use wildcards
    For copying and moving multiple files at the same time
    * You would use cp and mv commands.
      * ex: cp *.py ~/Documents
      * ex: mv *.py ~/Documents
* How to use brace expansion
    For creating entire directory structures in a single command
    * You would use mkdir -p and {}. 
      * ex: name/{F1,F2,F3}/{first,last}


