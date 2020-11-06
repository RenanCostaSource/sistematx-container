# IMAGEM
FROM mariadb

MAINTAINER Bruno Correia <brunogomescorreia@gmail.com>

COPY ./my.cnf /etc/mysql/my.cnf

ADD ./dump/* /docker-entrypoint-initdb.d/
