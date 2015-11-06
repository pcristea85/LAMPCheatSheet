# LAMPCheatSheet
A minimal cheatsheet with the most used commands (Ubuntu for now, more distros will be added)

#Linux

##File system Permissions
**chmod 755 -R path**
**chown -R owner:group file**

##Finding Files
##To find a file:

##To find a file anywhere on HD
**find path -name 'readme.txt' (recursive)**

##To find a file that contains a string

##Vim
**esc** to enter command mode

Find: /s
**q** to quit
**x** to save and exit
**i** to enter insert mode (edit mode)
**w** to save

#Apache 2
##View Enabled Modules
**apache2ctl -M**

##Installing modules
**sudo apt-get install**
##Enabling and disabling modules
**a2enmod**

#Mysql
Export DB
```mysqlexport -uusername -ppassword database_name path/exportedfile.sql```
Import DB: 
```mysql -uusername -ppassword database_name < path/filetoimport.sql```

#Archiving
##GZ
**tar xvzf file.tar.gz**
**tar xvzf file.tgz**

##ZIP

##RAR

#PHP
##Error Reporting
Where to find by order of importance.
XDebug config
	xdebug.force_display_errors
**php.ini** (usually in **/etc/php5/ [apache2 or cli] /php.ini**)
Note: CLI uses a separate ini
Note: There may be multiple ini files, to find the one being used, use **<?php phpinfo();?>**
httpd.conf
.htaccess
.php

Error Logging
Defined in php.ini
