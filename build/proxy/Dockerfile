FROM nginx

RUN rm /etc/nginx/conf.d/default.conf

COPY ./conf/app.template-nossl /tmp/

COPY ./conf/app.template-ssl /tmp/

COPY ./scripts/genAppNginx /usr/local/bin/

RUN chmod 777 -R /usr/local/bin/

RUN apt-get update && \
    apt-get install openssl -y

RUN openssl dhparam -out /etc/nginx/dhparam.pem 2048
