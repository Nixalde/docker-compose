FROM debian
#Instalacion de varnish
RUN apt -y update; /
apt -y install varnish

#Copia del fichero de configuracion
COPY /conf/default.vcl /etc/varnish/default.vcl

#Puerto de escucha de varnish
EXPOSE 80

#Arranque de varnish
ENTRYPOINT varnishd -f /etc/varnish/default.vcl -s malloc,1G
