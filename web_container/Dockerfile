FROM nginx:alpine

RUN rm /etc/nginx/conf.d/default.conf

COPY config/nginx.conf /etc/nginx/nginx.conf
COPY www/index.html /usr/share/nginx/html/

EXPOSE 80