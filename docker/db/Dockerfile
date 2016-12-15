# Version 0.0.2

FROM postgres:9.5

MAINTAINER Alex Mcknight <mcknight816@gmail.com>

#Allow Remote Connections
ADD init-settings.sh /docker-entrypoint-initdb.d/init-settings.sh
RUN chmod 755 /docker-entrypoint-initdb.d/init-settings.sh

ADD init-sql.sql /docker-entrypoint-initdb.d/init-sql.sql
RUN chmod 755 /docker-entrypoint-initdb.d/init-sql.sql