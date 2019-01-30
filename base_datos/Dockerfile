# Imagen que descargamos con "docker pull mariadb:latest"
FROM mariadb:latest
# Actualizamos el sistema
RUN apt-get update && \
    apt-get -y upgrade
# Establecemos variables de entorno
ENV MYSQL_ROOT_PASSWORD root
ENV MYSQL_DATABASE moodle_db
ENV MYSQL_USER moodle_user
ENV MYSQL_PASSWORD moodle
# Ejecutamos demonio de mariadb(mysql)
CMD ["mysqld"]