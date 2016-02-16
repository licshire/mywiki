#MariaDB

##官网
<http://mariadb.org/>

##安装 10.1
在/etc/apt/sources.list.d/中加入配置文件
```
sudo apt-get install mariadb-server

#运行如下命令，设定root密码及其他安全配置
mysql_secure_installation

#配置文件
/etc/mysql/my.cnf

#查看字符集
show variables like 'collation_%';
show variables like 'character_set_%';

#开启utf8
/etc/mysql/conf.d/mariadb.cnf
去掉注释后，重启服务
sudo service mysql restart
```

##命令
```
#查看版本
mysqladmin -u root -p version

#登陆到mysql
mysql -u root -p

#查看所有数据库 
show databases;

#创建数据库 
create database xxx;  

#删除数据库 
drop database xxx;

#查看数据库里面的表
use xxx;
show tables;
```

##备份和恢复
```
mysqldump -u root -p xxx > xxx.sql
mysql -u root -p xxx < xxx.sql
```