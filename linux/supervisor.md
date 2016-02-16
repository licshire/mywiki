#supervisor

##官网
<http://supervisord.org/>

##通过pip安装
```
pip install supervisor

cd /etc
mkdir supervisor
echo_supervisord_conf > /etc/supervisor/supervisord.conf

mkdir conf

#打开supervisord.conf
在文件最后加入
[include]
files = /etc/supervisor/conf/*.conf
```

##开机启动
从<https://github.com/Supervisor/initscripts>下载启动脚本
```
cp ubuntu /etc/init.d/supervisord

#可能需要修改supervisord、supervisorctl的路径

chmod +x supervisord

sudo update-rc.d supervisord defaults
```

##supervisorctl 命令
```
supervisorctl status

supervisorctl start xxx
supervisorctl stop xxx
#重新加载配置文件
supervisorctl reload
```