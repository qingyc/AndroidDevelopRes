下载安装

```
apt-get install nginx
RPM是RedHat Package Manager（RedHat软件包管理工具）类似Windows里面的“添加/删除程序”

阿里云服务ECS(CentOS7) 用yum源安装nginx

1、nginx地址： http://nginx.org/en/linux_packages.html#stable
安装源命令：
rpm -ivh http://nginx.org/packages/centos/6/noarch/RPMS/nginx-release-centos-6-0.el6.ngx.noarch.rpm
2、查看命令：
yum info nginx
3、安装命令：
yum install nginx
4、安装完成后nginx就已经启动了，可以查看进程：
ps -ef|grep nginx
5、关闭启动nginx
nginx -t 检查配置是否有误，并按照报错提示修复错误。
service nginx start
service nginx stop
```

配置

```
nginx 配置
目录 
linux 下 etc 

启动
使用以下命令即可解决：
nginx -c /etc/nginx/nginx.conf
1
nginx -s reload
1
其他命令： 
停止nginx服务：nginx -s stop
杀掉
[root@localhost ~]# killall -9 nginx
 ```