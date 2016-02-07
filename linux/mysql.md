#MySQL

##安装
sudo apt-get install mysql-server  

查看版本  mysqladmin -u root -p version  


登陆到mysql mysql -u root -p  
查看所有数据库 show databases;
创建数据库 create database wordpress;  
删除数据库 drop database wordpress;

###查看字符集
show variables like 'collation_%';  
show variables like 'character_set_%';  

配置文件位置 /etc/mysql/my.cnf
[client]  
default-character-set=utf8  
[mysqld]  
character-set-server=utf8  


启动 sudo service mysql start  
停止 sudo service mysql stop  


##备份和恢复
mysqldump -u root -p xxx > xxx_14.3.2.sql
mysql -u root -p xxx < xxx.sql