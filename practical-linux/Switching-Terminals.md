1. Switching Terminals
 Linux have 6 ttys by default, which we call as vcs & driver assigned to it <br>
is tty (/dev/tty*) <br>
To – switch from gui use CTRL ALT F1 & to switch between the terminals use <br>
ALT -F2, F3... <br>
To check current terminal use $ps command. <br>


`$df -h  ` - same as my computer in windows
`$fdsik -l` - list partition
`$man <cmd> ` - manual
`$clear ` - clear the screen
`$^l `  - -> clear the screen
`$ls`  -> list content
` $ls -l  `  -> list content in long listing format
` $ls -al  `  -> list all subcontent in long listing format
` $ll`   -> an alias for the above
`$ls -R` -> list content recursively
`$l.`  -> list hidden files
`$ls -F`  -> list content and classify them
`$alias`  -> display all aliases for current user
`$alias <statement>`  -> make alias eg alias c='clear'
`$unalias <alias>`   -> remove alias eg unalias c
`$exit`   -> log out from the system
`$logout`  -> log out from the system
`$^d`   -> log out from the system
`$tree`  -> list content in a tree (hierarchial) diagram
`$tree -d`  -> list subdirectories only - no files
`$tree -p`  -> list content with their permissions
`$cd <directory>`  -> change directory to...
`$cd .. `  -> change to parent directory
`$cd -`  -> change to previous directory
`$cd`  -> change to home directory
`$cd ~` -> change to home directory
`$pushd` -> change dir with pwd
`$cat` -> display a content of a file
`$pwd`  -> print work (current) directory
`$pwd -P`  -> print parent working dir of this symlink dir
`$mkdir <directory>`  -> make directory
`$mkdir -p <directory>`  -> make parent directories also if it does not exist
`$touch` -> make a 0 byte file if it does not exist
`$cp`  -> copy (for files)
`$cp -a`  -> copy (for directories)
`$cp -p`   -> copy and preserve date and time
`$mv`   -> move OR rename
`$rmdir` -> remove empty directory
`$rm` -> remove (for files)
`$rm -f`  ->removeforcefully ("")
`$rm -r`  -> remove recursively for directories 
`$rm -rf` -> remove recursively removeforcefully ("")
`$cat`  -> display content of the file 
`$cat -n` -> display content of the file and line number 
`$cal`   -> display calendar for current month
`$date` -> display system date and time
`$date -s `<value>``  -> change system date and time in mm/dd/yy
`$hwclock`   -> display the hardware clock
`$hwclock -hctosys`   -> set the system time from the hardware clock
`$ln -s`   -> make a soft/sym/symbolic link
`$ln`   -> make a hard link
`$history`  -> display the list of the last 1000 commands
`$! 100`   -> Run command 100 in history
`$vi`   -> text editor
`$vimtutor`  -> vi manual withexercise
`$pico` -> pico manual withexercise
`$mcedit` -> mcedit manual withexercise
`$joe`  -> joe manual withexercise
`$aspell -c <filename>`  -> check the spelling in the file
`$elinks`  -> check the web links
`$file` -> display the type of file
`$which`  -> display the path of binary 
`$whereis` -> display all paths
`$hostname` -> display system name with domain
`$id`  -> display id info of current user
`$id -u`  -> display user id of current user
`$id -un` -> display username of current user
`$id -g` -> display group id of current user
`$id -gn` -> display groupname of current user
`$uptime`  -> display for how long the system has been running
`$tty`  -> display current terminal number
`$users`  -> display no. of users currently logged in
`$whoami`  -> display username of current user
`$who`  -> display users logged in the system with their   respective terminals and time since logged in
`$who am i ' -> display current user, terminal and uptime
`$w` -> display is details which files are open on which terminal


http://www.oraclehome.co.uk/linux-commands.htm
$mkdir -p /opt/funny/test
$cd /opt/funny/test -- absolute path
$cd /opt/funny
$pwd
/opt/funny
$cd test –- relative path