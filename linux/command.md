#Linux常用命令

##删除
```
rm -f file  
rm -rf dir  
```

##重启、关机  
###重启  
```
shutdown -r now
```
###关机
```
shutdown -h now
```

##磁盘
```
df -h
```  

##进程
```
ps aux  
ps aux|grep xxx  
```

查看CPU和内存使用情况 
```
top

排序
x   进入高亮
shift + > 或 shift + <  改变排序
```  

##端口查看
```
netstat -h
netstat -ap

lsof
```

##用户
```
#默认主目录在/home/user
#-m 创建主目录
#-s 指定shell
useradd user -m -s /bin/bash
#设定密码
passwd user
```

##时间
```
#查看当前时间
date -R
#修改日期
date -s 2016-03-01
date -s 23:43
```

##查找文件
```
which xxx
whereis xxx
```

##内存占用
```
#按MB显示
free -m

#按人类可读方式显示
free -h
```
