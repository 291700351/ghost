FROM mysql:8.0.18
# Setting time zone
RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai' >/etc/timezone

# Setting root user password
ENV MYSQL_ROOT_PASSWORD=99233123

EXPOSE 3306

VOLUME [ "/var/lib/mysql"]