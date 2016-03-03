#ubuntu
<http://www.ubuntu.com/>

##版本
```
uname -a
lsb_release -a
```

##启动管理
```
sudo apt-get install sysv-rc-conf
```

##git 
``` 
sudo apt-get install git
```

##临时进入root模式
```
sudo -i
```

##开发环境
```
sudo apt-get install build-essential
```

##服务
```
#前提是在/etc/init.d目录下有启动脚本
#添加一个服务
sudo update-rc.d ServiceName defaults
#删除一个服务
sudo update-rc.d ServiceName remove
```

##时区
```
sudo tzselect
sudo cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime


```

##硬件信息
CPU   cat /proc/cpuinfo  


##ulimit -a
* 在文件/etc/security/limits.conf中增加  
  * hard nofile 40960
  * soft nofile 40960
* 在文件/etc/profile加上一行 ulimit -SHn 40960  