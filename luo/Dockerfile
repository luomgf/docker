#this is comment
#指定基镜像
FROM	ubuntu:12.04
MAINTAINER      Docker luomgf <luomgf@163.com>  #维护者信息
RUN     apt-get -qq update      #创建时执行安装
RUN     apt-get -qqy install ruby       ruby-dev
#将物理主机中文件复制到docker /var/www
ADD     add_myfile      /var/www
#向外部开放80端口
EXPOSE 80
#默认容器启动后启动程序
CMD ["/usr/sbin/apachectl","-D","FOREGROUND"]
