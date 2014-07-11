title: sql-quick-sheet
date: 2014-02-01 17:30:07
tags: sql
---
CommonSQL for the common developer


What's my hostname?
``` sql
select @@hostname;
show variables where Variable_name like '%host%';
```
use sql through vagrant as root, login
source: https://coderwall.com/p/yzwqvg
``` shell
mysql -u root -e "GRANT ALL PRIVILEGES ON *.* TO 'root'@'%' IDENTIFIED BY '' WITH GRANT OPTION; FLUSH PRIVILEGES;"

cat /etc/mysql/my.cnf | grep bind-address

```

Pick a database
``` sql
use databaseNAME
```

AutoComplete for mysql commands
``` sql
mysql --auto-rehash -u root -p
```

Create a table 
``` sql
CREATE TABLE users
(
ID int NOT NULL AUTO_INCREMENT,
FirstName varchar(255),
PRIMARY KEY (ID)
)
```
insert into table
``` sql
insert into users (ID, FirstName) values (null, 'bob');
```