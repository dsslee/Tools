# Shell Commands

## 목차

* 1. [Most Commonly Used](#1-most-commonly-used)
* 2. [Booting & Shutdown](#2-booting-shutdown)
* 3. [Manipulating Files and Directories](#3-manipulating-files-and-directories)
* 4. [Combining Tools](md#4-combining-tools)

## 1. Most Commonly Used
|Command|Description|
|--|--|
|history|-|
|history <#>|-|
|history -c|clear history|
|history -w  <file name>|save command to file|
|man <command>|-|
|man -k <command>|short manual|
|<command> -- help|-|
|locate <file name>|-|
|watch -d -n 0.5 nvidia-smi|


## 2. Booting & Shutdown
|Command|Description|
|--|--|
|reboot|system reboot|
|reboot -f|force system reboot|
|halt|system shutdown|
|halt -f|force system shutdown|
|shutdown -h now|shutdown now|
|shutdown -h 10|shutdown after 10min|
|shutdown -h 15:10|shutdown at 15:10pm|
|shutdown -r now|system rebookt now|
|shutdown -c|cancel scheduled shutdown|
|init 0|Runlevel0 |
|init 1|-|
|init 2|-|
|init 3|-|
|init 4|-|
|init 5|-|
|init 6|-|


## 3. Manipulating files and directories
|Command|Description|
|--|--|
|pwd|print working directory|
|ls|listing|
|cd|change directory|
|~ |home directory|
|ls ~|list home directory|
|cd ~ |home|
|cp original copy|copy|
|mv|move|
|mv|rename file|
|rm|remove file|
|rmdir|removes directory when folder is empty|
|mkdir|makes directory|
|ls -R -F|list everything in the directory|
|man command|manual|
|history|lists history of commands|
|!command|rerun command|> |output file|

## 4. Combining Tools
|Command|Description|
|--|--|
|>|ouputs into a file|
|\| |use output of hte command on the left as hte input to the command on the right|
|wc|word count <br> - c byte count <br> - l newline count <br> - w word count|
|*|wildcard|
|?|match single character|
|[..]|match any one of the characters inside the square brackets|
|{..}|match any of the comma separated patterns inside curly brakcet|
|sort|- r reverse <br> - n numeric sort|
|uniq|remove adjacent duplicated lines|
|ctrl + c|stop running program|
