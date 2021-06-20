FROM mariadb
ENV MYSQL_ROOT_PASSWORD qhdks100!
ENV MYSQL_DATABASE MYSQL_DATABASE
COPY ./mysql_data/mysql /var/lib/mysql
EXPOSE 3306
ENTRYPOINT ["mysqld", "--user=root"]