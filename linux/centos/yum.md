#yum

##配置文件目录
```
/etc/yum.repos.d
```

##命令
* yum check-update   //列出可更新软件
* yum --security check-update   //安全更新,可能需要 yum install yum-security
* yum update //更新软件
* yum update --security  //只安装安全更新
* yum install xxx  //安装xxx
* yum search xxx   //查找xxx
* yum remove xxx  //删除xxx
* yum info xxx   //xxx的相关信息

清除缓存
yum clean all

##国内镜像
[国内镜像](../mirrors.md)