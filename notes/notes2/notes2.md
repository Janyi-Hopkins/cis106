---
name : Ja'nyi Hopkins Walker
semester : spring 24
course : cis106
---

# Notes 2
[Presentation](https://rapurl.live/s39)
[Article](https://cis106.com/extra/thelinuxfs/)


## Commands used for navigating the file system:

## pwd
### Definition
Used for displaying the current working directory
### Usage
`pwd`
### Examples
* Print the absolute path of your current working directory 
  * `pwd`

## cd 
### Definition
Used for changing the current working directory
* when no specific directory to change to is given (cd ) it will bring you to the home directory
### Usage
`cd` + `destination`
### Examples
* Will bring you to your home directory
  * `cd`
* Will bring you to the previous working directory
  * `cd -`
* Will bring you back one step in a directory 
  * `cd ../`
* Will bring you to your downloads directory
  * `cd Downloads/`

## ls
### Definition
Used for displaying all the files inside a given directory 
* when no directory is given ls displays the files in the current working directory
### Usage
`ls` + `option` + `directory to list`
### Examples
* list your current working directory
  * `ls`
* list all files including the hidden files
  * `ls -a`
* list all the files inside a given directory
  * `ls -a ~/Pictures`



## Definitions of the following terms:

* **File System**
  * The way the files are stored and organized.

* **Pathname**
  * The location of a given file in your computer, also known as file path. The path can be relative or absolute.

* **Absolute Path**
  * The location of the file starting at the root of the file system. For example, `/home/maria53/Downloads/list.txt`.

* **Relative Path**
  * The location of the file starting from a child directory of the current working directory. For example, assuming the current working directory is `/home/maria53` the relative path would be `Downloads/list.txt`.

* **Your Home vs. The Home**
  * Your Home directory is the user's personal directory where all your files are located, every user has their own. The home directory is the parent directory of all the home directories, this is where all the users' home directories are.

* **Parent Directory**
  * A directory containing one or more directories and files

* **Child Directory or Subdirectory**
  * A directory inside another directory.

* **Bash Special Characters**
  * They function like commands that tell the shell to perform a specific action without having to type the complete command.

* **Environment Variables**
  * They store values of a user's environment and can be used in commands in the shell. The values can be unique to the users' environment.

* **User Defined Variables**
  * They are variables created by the user and exist only in the script and subshell that runs the script. Allow you to temporarily store data and be used throughout the script.

* **Why do we use $ with variables in bash shell scripting?**
  * We use $ with variables in bash shell scripting so that we can use the value stored in the variable.