查询mysql进程
```
ps -ef | grep mysql
```

连接mysql
```
/usr/local/mysql/bin/mysql -uroot -h xxx.xxx.xxx.xxx -p
```

复制table
```
/usr/local/mysql/bin/mysqldump -h xxx.xxx.xxx.xxx database table -uroot  -p > table.sql
```

复制table(database)
```
/usr/local/mysql/bin/mysqldump -h xxx.xxx.xxx.xxx database  -uroot  -p > database.sql
```

查询文本生成新文件
```
 grep "220.181.102.176" /Users/cuitianze/Downloads/tmp2 > 220.181.102.176
```

安装mysql-shell (https://bugs.mysql.com/bug.php?id=81051)    
enable the mysql-tools-preview repository
```
vim /etc/yum.repos.d/mysql-community.repo
```
```
[mysql-tools-preview]
name=MySQL Tools Preview
baseurl=http://repo.mysql.com/yum/mysql-tools-preview/el/6/$basearch/
enabled=1
gpgcheck=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql
```
```
yum install mysql-shell
```
```
mysqlsh -u root -h localhost -p --classic --dba enableXProtocol
```

导入数据库
```
mysqlsh -u root --sql --recreate-schema tougudashi < tougudashi.sql
```

允许外网访问
```
mysql> use mysql;
mysql> select host, user from user;
mysql> update user set host = '%' where user = 'root';
mysql> FLUSH PRIVILEGES;
```
```
mysql> GRANT ALL PRIVILEGES ON *.* TO 'cuitianze'@'114.240.245.12' IDENTIFIED BY 'Cuitianze@123' WITH GRANT OPTION;
```
