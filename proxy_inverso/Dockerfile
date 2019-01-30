FROM debian
#Instalacion de varnish
RUN apt -y update; /
apt -y install varnish

#Copia de los ficheros de configuracion
COPY /conf/varnish /etc/default/varnish
COPY /conf/varnish.service /lib/systemd/system/varnish.service
COPY /conf/default.vcl /etc/varnish/default.vcl

#Puerto de escucha de varnish
EXPOSE 80

#Arranque de varnish
ENTRYPOINT varnishd -f /etc/varnish/default.vcl -s malloc,1G
