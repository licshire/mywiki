##安装
sudo apt-get install nginx  

##配置  
/etc/nginx/

##启动和停止
sudo /etc/init.d/nginx start  
sudo /etc/init.d/nginx stop

##配置
nginx.conf  
server_tokens off;  

fastcgi_params  
fastcgi_param   SERVER_SOFTWARE         nginx;