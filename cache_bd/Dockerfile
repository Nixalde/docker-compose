# Imagen que descargamos con "docker pull mariadb:latest"
FROM mariadb:latest
# Actualizamos el sistema
RUN apt-get update && \
    apt-get -y upgrade
# Establecemos variables de entorno
ENV MYSQL_ROOT_PASSWORD root
ENV MYSQL_DATABASE moodle_db

#Activamso la caché

COPY /conf/cache.sql /tmp/cache.sql

RUN "mysql -u root --password="root" moodle_db < /tmp/cache.sql"