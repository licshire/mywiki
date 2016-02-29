参考：<http://www.cnblogs.com/JemBai/archive/2009/03/19/1416364.html>

```
#查看当前防火墙规则
service iptables status
#查看filter表
iptables -L
#查看nat表
iptables -t nat -L
 
 
#防火墙规则
iptables -F
#nat 清除  iptables -F -t nat
 
iptables -A INPUT -p tcp --dport 22 -j ACCEPT
iptables -A INPUT -p tcp --dport 80 -j ACCEPT
iptables -A INPUT -i lo -j ACCEPT
iptables -A INPUT -p icmp -j ACCEPT
iptables -A INPUT -m state --state ESTABLISHED,RELATED -j ACCEPT
 
iptables -P INPUT DROP
iptables -P FORWARD ACCEPT
iptables -P OUTPUT ACCEPT
 
#保存规则
service iptables save
 
#重启iptables 
service iptables restart
#删除某条规则，先查出行号
iptables -L --line-number
#删除行号2的规则
iptables -D INPUT 2
```