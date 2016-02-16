#防火墙ufw

##安装
```
sudo apt-get install ufw
```

##命令
```
#查看防火墙状态 
sudo ufw status

#开启防火墙 
sudo ufw enable

#默认不能访问所有
sudo ufw default deny

#允许端口访问
sudo ufw allow 22

#删除掉允许
sudo ufw delete allow 22

#关闭
sudo ufw disable
```