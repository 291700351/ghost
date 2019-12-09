# 根据mysql 8.0.18镜像构建我们自己的镜像
FROM mysql:8.0.18
# 设置容器时区,docker容器迷人时区不是东八区，所以手动设置一下，避免出现时区不对，导致时间差错
RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai' > /etc/timezone
# 设置镜像中mysql root用户的密码
ENV MYSQL_ROOT_PASSWORD=123456
# 端口3306
EXPOSE 3306
# mysql数据
VOLUME [ "/var/lib/mysql"]