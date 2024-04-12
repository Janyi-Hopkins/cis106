---
name : Ja'nyi Hopkins Walker
semester : spring 24
assignment : notes 4
---

# Notes 4

## Wildcards

## * Wildcard
the * wildcard matches from 0 to any number of characters.
* Examples:
  * list all txt files in the directory
    * 'ls *.txt '
  * list all files that start with the word file
    * 'ls file* '
  * Copy all the mp4 files
    * 'cp Downloads/*.mp4 ~/Videos/Movies/ '

## ? Wildcard
the ? wildcard matches only one character
* Examples:
  * list all hidden files in current directory
    * 'ls ./.??* '
  * list all hidden files in the parent directory
    * 'ls ../.??* '
  * list all files that have two characters between letter b and k
    * 'ls b??k* '

## [] Wildcard 
the {} wildcard match a single character in a range
* Examples:
  * match all files that have a vowel after letter f
    * 'ls f[aeiou]* '
  * match all files that do not have a vowel after letter f
    * 'ls f[!aeiou]* '
  * match all files whose name begins with any 3 combinations of numbers and the current user's username
    * 'ls [0-9][0-9][0-9]$USER '

## Brace Expansion
Brace expansion is not a wildcard but another feature of bash that allows you to generate arbitrary strings to use with commands.
* Examples:
  * create a whole directory structure in a single command
    * mkdir -p music/{jazz,rock}/{mp3files,videos,oggfiles}/new{1..3}
  * create N number of files
    * touch website {1..5}.html
  * remove multiple files in a single directory
    * rm -r {dir1,dir2,dir3,file.txt,file.py}