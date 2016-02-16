#ubuntu
<http://www.ubuntu.com/>

##版本
```
lsb_release -a
```

##启动管理
```
sudo apt-get install sysv-rc-conf
```

git  
sudo apt-get install git  
开发环境  
sudo apt-get install build-essential  
后台服务管理(设定/etc/init.d/ 下面的命令是否开机启动)  


##硬件信息
CPU   cat /proc/cpuinfo  

##防火墙ufw
开启SSH端口 sudo ufw allow ssh  
开启80端口 sudo ufw allow http  
默认外部不能访问所有端口 sudo ufw default deny  
开启防火墙 sudo ufw enable  
查看防火墙状态 sudo ufw status  

##ulimit -a
* 在文件/etc/security/limits.conf中增加  
  * hard nofile 40960
  * soft nofile 40960
* 在文件/etc/profile加上一行 ulimit -SHn 40960  