# LAMP Stack
# https://github.com/s-n-n/lamp
Provides customizable LAMP stack.

It includes:
 * PHP 7.1.3, from official docker images, both can run at the same time, on different ports
 * mysql 5.7.30 database
 * mysql data files are stored on db_data folder

## Run with:

Enter folder .docker and run `docker-compose up -d` to start the stack.

## mysql
docker exec -it docker_db_1 /bin/bash
mysql -uroot -ptoor DBNAME < /var/lib/mysql/dump.sql
mysqldump -uroot -ptoor DBNAME | gzip > /var/lib/mysql/dump.sql.gz

To be continued.