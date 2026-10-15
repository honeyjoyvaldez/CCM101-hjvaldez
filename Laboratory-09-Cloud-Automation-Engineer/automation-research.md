# Research: The Language of Automation

## Bash Script
A Bash script is a plain-text file containing a series of shell commands executed sequentially by the Unix/Linux command interpreter. The `#!/bin/bash` line at the very top is called a "shebang," which instructs the operating system which interpreter program to use to execute the instructions within the script file.

## Variables
Programmers use variables (such as `$BACKUP_DIR`) to store and reuse data dynamically instead of hardcoding exact folder paths throughout the script. This practice ensures maintainability, making it simple to update parameters in one central location rather than changing multiple lines of code.

## Cron Job
A cron job is a time-based task scheduler native to Unix-like operating systems that automatically runs commands or scripts at designated times, dates, or intervals. It is essential for cloud operations because it eliminates manual intervention for repetitive administrative routines like system updates and automated backups.
