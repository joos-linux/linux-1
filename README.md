# linux-command
Simple command (ubuntu)

# 1 Lesson

- uptime - system time / work
- uname - about system
- uname -a - about system all
- lscpu - system hardware
- ls - list directory contents
- ls -l - show more
- echo $PATH - programm path
- echo Hello World - write Hello World
- man -k time - show all command with time
- man uptime - show uptime manual
- in man - q - quit, h - help, /word - find word
- info uptime - show info uptime
- whatis uptime - show short info uptime
- whereis uptime - show uptime path (only system file)
- locate uptime (or readme.txt) (only system file?)
- ps - show process
- ctrl + z - background process (ping)
- fg - show bsckground process
- ctrl + c - stop process
- ls -la -R / -show all files, directories

### 2 Lesson --------------------

- cd / - move to directory
- ls -la - show description + hidden file
- pwd - print working directory
- cat text.txt - read text
- more text.txt - read text
- less text.txt - read text
- touch file.txt (not exist) - create file
- touch dir/file (exist) - change file/dir time
- cp test.txt /home/user/ - copy file/dir
- cp -v - verbose - show copy
- cp -R - recursive - copy file in directory to other directory
- rm test.txt - remove
- mv test.txt .text.txt - move/rename

### 3 Lesson --------------------

- mkdir - make dir
- mv dir1 newdir1 - move dir
- rmdir dir1 - rm empty dir
- rm -R dir1 - rm all dir
- cp dir1 dir4 - copy dir
- ln -s(symbolic link) /home/user/Dociments/dir1 MyLinkDir - make symbolic link dir
- ln -s file.txt MyFile.txt - make symbolic link file 
- ln file.txt fileDuplicate - make duplicate (only file)
- find /home(where) -name "*.txt*" -  find all txt-file in home-directory
- find / -name readme.txt - find readme in /
- wc test.txt - show (-w) words, (-l) lines, symbols
- sort - names.txt - show sort names in file
- sort -n numbers.txt - show sort numbers in file (sort num (1,2,11) not symbols(1,11,2))
- cut -d ">" (<-delimeter) -f 3 (number column) example.txt - show only 3. column in file
- cut -d ">" -f 3 example.txt | sort | wc - show and sort
- | - pipe - send output farther

### 4 Lesson --------------------

- grep linux (what) ./* (who) - find file with word linux in direcory
- 
