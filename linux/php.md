#PHP

sudo apt-get install php5-fpm  
sudo apt-get install php5-mysql  

#配置文件
```
listen = 127.0.0.1:9000
listen = /var/run/php5-fpm.sock
```
配置文件修改/etc/php5/fpm/php.ini  
不在http头中输出php版本号  
expose_php = Off  