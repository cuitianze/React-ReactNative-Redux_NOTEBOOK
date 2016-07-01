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
