FROM nginx

COPY ./conf/default.conf /etc/nginx/conf.d/default.conf

RUN apt-get update && \
    apt-get install certbot -y
