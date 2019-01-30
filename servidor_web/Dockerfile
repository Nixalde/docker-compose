FROM nginx:1.15
EXPOSE 8080
COPY /conf/index.html /usr/share/nginx/html
COPY /conf/nginx.conf /etc/nginx/
COPY /conf/site.conf /etc/nginx/conf.d
ENTRYPOINT nginx
