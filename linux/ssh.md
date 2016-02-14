#ssh

##ssh
ssh 用户名@IP地址
ssh -p 新端口 用户名@IP地址

##sftp
sftp 用户名@IP地址
sftp -o port=新端口 用户名@IP地址

##无密码登录
```
#在~/.ssh目录中生成id_rsa.pub和id_rsa
ssh-keygen

#关键权限
chmod 700 .ssh
chmod 600  authorized_keys

#authorized_keys中加入需要登录到本机的id_rsa.pub  

#配置/etc/ssh/sshd_config，只能使用秘钥登陆，不能通过输入密码登陆
PasswordAuthentication no

#修改ssh的端口为XXXX
Port XXXX

#关闭root登陆
PermitRootLogin no

#关闭空密码登陆
PermitEmptyPasswords no

#去掉下面3句的注释
RSAAuthentication yes
PubkeyAuthentication yes
AuthorizedKeysFile      .ssh/authorized_keys

#重启sshd服务(centos7)
systemctl restart sshd.service
```

