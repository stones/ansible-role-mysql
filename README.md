Ansible Mysql Role
==============
***Ubuntu Only (currently)***

In order securely access a MYSQL database, this role install mysql app and creates a root user.

#### Excute
In you main yaml file add, under roles:

```
- mysql
```

#### Steps taken
- Install Mysql packages( server, client python-mysqldb )
- Start MYSQL
- Add root user
- create a .my.cnf to allow root to connect without prompt
- Removes test database

#### Variables required

Example:

```
mysql_root_user: admin	
mysql_root_user: root
```

#### Todo
- Make multi-distribution
