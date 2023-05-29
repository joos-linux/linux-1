# linux-command
Simple command (ubuntu)

# 1 Lesson

- df - check memory
- df -h /dev/sda2 - check sda2
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
- cat /proc/meminfo - Memory info
- du -sh /Desktop - Desktop size
- ss -tulpn - open ports

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
- grep -i (ignore key sensitive) linux ./*
- grep .gov mydata.doc - find string with .gov in file
- grep -E(regexp) "[A-Za-z\.]*@*[A-Za-z].gov" mydata.doc - find pattern (email .gov) in file
- [A-Z]* - capital letters
- [0-9]* - numbers
- [A-Za-z]*@*[A-Za-z]*.com - email
- www\.[a-z]*\.com - web adress
- ' > - sent output
- sort names.txt > names_sortes.txt
- ' >> - append output
- sort numbers >> names_sorted.txt
- sort names.txt > names.txt - erase file (because first make names.txt then sort empty file)
- 2> error stream
- grep joos /etc/* 2> errors.txt - send errors (permission denied) to errors.txt
- grep joos /etc/* 2> /dev/null - send errors to null
- grep joos /etc/* > good/.txt 2> nogood.txt - separation good and nogood output
- &> - > + 2> - to 1 file

### 5 Lesson --------------------

- tar cvf(create verbose file) mytar.tar folder1 - tar folder1 ro mytar
- tar tf(test file) mytar.tar - look inside mytar
- tar xvf(extract verbose file) mytar.tar - extract tar
- gzip  bzip2 xz - compression file command
- gzip mytar.tar - make mytar.tar.gz and compress
- gunzip mytar.tar.gz - unzip
- bzip2 / bunzip2 - compress, decompress
- xz / unxz - compress, decompress
- tar cvzf(zip-compress) myzip.gz Folder1 - tar + gzip compress
- tar cjf(j - bzip2) mybzip.bz2 Folder1
- tar cJf(J -xz) myxz.xz Folder1
- tar xvf myzip.gz (mybzip.bz2 myxz.xz) - extract
- zip -r myzip.zip Folder1
- unzip myzip.zip

### 6 Lesson --------------------

- top - task manager / cpu / task / Mem
- schift P - sort processors, schift M - sort Memory
- free - memory use
- free -h - human memory use
- ps - user process
- ps -u joos - all joos process
- ps -aux - all users process
- cd /var/log - all logs
- dmesg - kernel log
- nano file.txt  Ctrl + O / Ctrl +  X
- vi
- i - write
- Esc - end write
- :w - save
- :q - quit
- :wq!(! - disable errors) vi.txt - save vi.txt quit

### 7 Lesson --------------------

- cat /etc/passwd - users
- cat /etc/shadow - password list
- cat /etc/group - groups with user
- whoami - show who user now
- id user1 - show user1-id, groups-id
- last - last system login
- who - who is now in system
- w - who is on and what do
- useradd -m user1 - add user1 with home directory
- passwd user1 - update password user1
- cd /etc/skel - template for user home directory
- userdel -r user1 - remove user and group
- userdel user1 - remove only user
- groupadd group1 - add group
- groupdel group1 - remove group
- usermod -aG(add group) group1 user1 - add user1 to group1
- deluser user1 group1 - remove user1 from group1

### 8 Lesson --------------------

- chown user2 dir123 - change owner(user2) dir123
- chgrp group2 test.txt change group(group2) text.txt
- chmod o+x text.txt - change rights (add x) for other (o)
- chmod g-w text.txt - change rights (del w) for group (g)
- chmod g-w,o+w text2.txt
- chmod ugo(or a=all)=r text.txt - change rights user+group+other = read
- r = 4 w = 2 x = 1
- chmod 777 text.txt
- chmod o+t mydir - add sticky bit - only owner can delete in folder
- chmod o-t mydir = chmod 1777 mydir
- ifconfig / ip a
- ip addr show
- route
- ip route show
- ping
- ping -c 4
- traceroute
- host www.ebay.com - show ip(info) about website
- dig www.ebay.com - show info about website
- netstat - show ports
- wget (link from internet) - download from internet
### Ubuntu Debian
- apt-get install openssh-server - install software
- whereis openssh-server
- apt-get remove openssh-server - remove software
- cat /etc/apt/sources.list - repositories
- dpkg -i (install) package-name.deb - install .deb
- dpkg -r (remove) package-name - remove package
### RedHat Centos
- yum install inkscape - install inkscape
- yum remove inkscape - remove inkscape
- rpm -i (install) nethack.rpm - install .rpm
- rpm -e (erase) nethack - erase .rpm
- reboot now
- shutdown now
