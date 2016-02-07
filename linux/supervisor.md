#supervisor

##安装
[setuptools](https://pypi.python.org/pypi/setuptools/)  
easy_install supervisor  
sudo cp supervisord.conf /etc/
sudo mkdir /etc/supervisord.conf.d  

启动脚本放到/etc/init.d/下  
sudo cp supervisord /etc/init.d/  