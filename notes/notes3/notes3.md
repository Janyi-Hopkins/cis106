---
name : Ja'nyi Hopkins Walker
semester : spring 24
course : cis106
---

# Notes 3

## Managing Files and Directories

## mkdir
### Definition 
Used to create single or multiple directories.
### Usage
`mkdir` + `name of directory`
### Examples
* create a directory in present working directory
  * `mkdir wallpapers`
* create a directory in a directory using relative path
  * `mkdir wallpapers/ocean`
* create a directory with a space in the name
  * `mkdir wallpapers/new\ cars`

## touch
### Definition 
Used for creating files.
### Usage
`touch` + `name of file`
### Examples
* to create a file called list
  * `touch list`
* to create several files
  * `touch list_of_cars.txt script.py names.csv`
* create a file with a space in its name
  * `touch "list of foods.txt" `

## rm
### Definition 
Used to remove files or non empty directories
### Usage
`rm` + `file name`
### Examples
* remove a file
  * `rm list`
* remove a file and prompt confirmation before removal
  * `rm -i list`
* remove all the files inside a directory and ask before removing more than 3 files
  * `rm -I Downloads/games/* `
  
## rmdir
### Definition 
Remove empty directories
### Usage
`rm` + `name of directory`
### Examples
* remove an empty directory
  * `rmdir Downloads/games`

## mv
### Definition 
Moves and renames files and directories
### Usage
* moving directories
  * `mv` + `source` + `destination` 
* renaming directories
  * `mv` + `file/directory to rename` + `new name`
### Examples
* to move a file
  * `mv Downloads/homework.pdf Documents/`
* to move a directory from one directory to another using absolute path
  * `sudo mv ~/Downloads/theme /usr/share/themes`
* to rename a file
  * `mv homework.docx cis106homework.docx`

## cp
### Definition 
Copies file and directories from a source to destination
### Usage
* to copy files
  * `cp` + `files to copy` + `destination`
* to copy directories
  * `cp` + `-r` + `directory to copy` + `destination`
### Examples
* to copy a file
  * `cp Downloads/wallpapers.zip Pictures/`
* to copy content of a directory to another directory
  * `cp Downloads/wallpapers/* ~/Pictures/`
* to copy multiple files in a single command
  * `sudo cp -r script.sh program.py home.html assets/ /var/www/html/`

## file
### Definition 
Determines the type of file
### Usage
`file` + `name of file`
### Examples
* display file type
  * `file filename`
* display file type without file name
  * `file -b filename`

## pdfinfo
### Definition 
Displays information about pdf files
### Usage
`pdfinfo` + `name of file.pdf`
### Examples
* display info of a file
  * `pdfinfo filename.pdf`

## mediainfo
### Definition 
Command line tool to display information about audio/video files
### Usage
`mediainfo` + `name of file`
### Examples
* display information about a media file
  * `mediainfo example.png`
* display full information of a media file
  * `mediainfo -f example.png`
* output information to an html file
  * `mediainfo --output=HTML example.png > file.html`

## exiv2
### Definition 
Image metadata manipulation tool
### Usage
`exiv2` + [option] + [action] + [file]
### Examples
* Displays information about an image file
  * `exiv2 example.png`
* Displays all exif data about an image file
  * `exiv2 -pt example.png`

## exiftool
### Definition
Read and write meta information in files
### Usage
`exiftool` + `path or name of file`
### Examples
* displays information about a file
  * `exiftool example.png`