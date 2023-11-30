---
name : Ja'nyi Hopkins Walker
semester : fall 23
course : cis106
---

# Week Report 7

## Commands 

### Cat 
* What is the command used for?
  * The cat command is used for displaying the content of a file.
* What is the formula of the command?
  * The formula is : cat + option + file(s) to display
* Examples
  * example 1:
    * display the content of a file located in the pwd : cat todo.lst
  * example 2:
    * display the content of a file using absolute path : cat ~/Documents/todo.lst
  
### Tac
* What is the command used for?
  * The tac command is used for displaying the content of a file in reverse order.
* What is the formula of the command?
  * The formula is : tac + option + file(s) to display
* Examples
  * example 1:
    * display the content of a file located in the pwd : tac todo.md
  * example 2:
    * display the content of a file using absolute path : tac ~/Documents/todo.md

### Head
* What is the command used for?
  * The head command is used for displaying the top N number of lines of a given file.
* What is the formula of the command?
  * The formula is : head + option + file(s)
* Examples
  * example 1:
    * Display the first 10 lines of a file : head ~/Documents/Book/dracula.txt
  * example 2:
    * Display the first 5 lines of a file : head -5 ~/Documents/Book/dracula.txt

### Tail 
* What is the command used for?
  * The tail command is used for displaying the last N number of lines of a given file.
* What is the formula of the command?
  * tail + option + file
* Examples
  * example 1:
    * Display the last 10 line of a file : tail ~/Documents/Book/dracula.txt 
  * example 2:
    * Display the last 5 lines of a file : tail -5 ~/Documents/Book/dracula.txt

### Cut 
* What is the command used for?
  * The cut command is used for extracting a specific section of each line of a file and display it to the screen.
* What is the formula of the command?
  * The formula is : cut + option + file(s)
* Examples
  * example 1:
    * Display a list of all the users in your system : cut -d ':' -f1 /etc/passwd
  * example 2:
    * Display a list of all the users in your system with their login shell : cut -d ':' -f1,7 /etc/passwd
  
### Paste 
* What is the command used for?
  * The paste command is used for joining files horizontally in columns.
* What is the formula of the command?
  * The formula is : paste + options + files
* Examples
  * example 1:
    * merge two files : paste users.lst ip_address.lst
  * example 2:
    * Merge two files using a different delimiter : paste -d ":" users1.lst ip_addresses.lst

### Sort 
* What is the command used for?
  * The sort command is used for sorting files.
* What is the formula of the command?
  * The formula is : sort + option + file
* Examples
  * example 1:
    * Sort a file : sort users.lst
  * example 2:
    * Sort a file in reverse order : sort -r users.txt

### Wc 
* What is the command used for?
  * The wc command is used for printing the number of lines, characters, and bytes in a file.
* What is the formula of the command?
  * The formula is : wc + option + file(s)
* Examples
  * example 1:
    * Display the number of characters in a file : wc -m users.txt
  * example 2:
    * Display the number of lines in a file : wc -l users.txt
  
### Tr 
* What is the command used for?
  * The tr command is used for translating or deleting characters from standard output.
* What is the formula of the command?
  * The formula is : Standard output | tr + option + set + set
* Examples
  * example 1:
    * Translate white space into tabs : cat program.py | tr "[:space:]" '\t'
  * example 2:
    * Translate tabs into space : cat file.py | tr -s "[:space:]" ' '

### Diff
* What is the command used for?
  * The diff command is used for comparing files and displays the differences between them. 
* What is the formula of the command?
  * The formula is : diff + option + file1 + file2
* Examples
  * example 1:
    * Display the difference between two files : diff cars.csv cars-backup.csv
  * example 2:
    * Display the difference between two files in a column format : diff -y cars.csv cars-backup.csv
  
### Grep 
* What is the command used for?
  * The grep command is used for searching text in a given file. 
* What is the formula of the command?
  * The formula is : grep + option + search criteria + file(s)
* Examples
  * example 1:
    * Search any line that contains the word "dracula" in the given file : grep 'dracula' ~/Documents/dracula.txt
  * example 2:
    * Search any line that contains the word "dracula" regardless of the case : grep -i 'dracula' ~/Documents/Books/dracula.txt

### Awk 
* What is the command used for?
  * Awk is a scripting language used for processing and displaying text.
* What is the formula of the command?
  * The formula is : awk + options + {awk command} + file + file to save (optional)
* Examples
  * example 1:
    * Print the first column of every line of a file : awk '{print $1}' ~/Documents/Csv/cars.csv
  * example 2: 
    * Print the first field of /etc/passwd file : awk -F: '{print $1}' /etc/passwd
  * example 3: 
    * Print the last field of the /etc/passwd file : awk -F '{print $NF}' /etc/passwd
  * example 4:
    * Print the first and last field of the /etc/passwd : awk -F: '{print $1," = ",$NF}'
  * example 5:
    * Print the first and 3rd field with line numbers : awk -F: '{print NR,$1,$3}' /etc/passwd

### Sed 
* What is the command used for?
  * The sed command is a stream editor that performs operations on files and standard output.
* What is the formula of the command?
  * The formula is : sed options + sed script + file
* Examples
  * example 1:
    * Replacing a string in given file (replace pizza with rice) : sed 's/pizza/rice/' shopping-list.lst
  * example 2:
    * Replacing the number of occurrences of a pattern in a file : sed 's/pizza/rice/4' shopping-list.lst
  * example 3:
    * Replacing all the occurrences of the pattern in a file : sed 's/pizza/rice/g' shopping-list.lst
  * example 4:
    * Replacing string on a specific line number : sed '3 s/pizza/rice/' shopping-list.lst
  * example 5: 
    * Replacing string on a range of lines : sed '1,3 s/pizza/rice/' shopping-list.lst
