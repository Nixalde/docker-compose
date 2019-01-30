FROM nginx:1.15
EXPOSE 8080
COPY /conf/index.html /usr/share/nginx/html/index.html
COPY /conf/nginx.conf /etc/nginx/nginx.conf
COPY /conf/site.conf /etc/nginx/conf.d
ENTRYPOINT nginx
