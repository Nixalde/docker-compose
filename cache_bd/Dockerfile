# Descargamos la imágen
#FROM mariadb:latest
# Establecemos variables de entorno
#ENV MYSQL_ROOT_PASSWORD root
#ENV MYSQL_DATABASE moodle_db

#Activamos la caché

COPY /conf/cache.sql /tmp/cache.sql

RUN "mysql -u root --password="root" moodle_db < /tmp/cache.sql"
