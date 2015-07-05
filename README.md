# MySQL Dump Docker

A simple docker image to dump MySQL (or MariaDB) databases to a target directory.

This is most useful when linking to another container, and when the destination directory is part of a backup strategy.

`docker run --rm --link=myMysqlServer:mysql -e MYSQL_HOST=mysql -e MYSQL_PASSWORD=password joshbenner/mysql-dump`