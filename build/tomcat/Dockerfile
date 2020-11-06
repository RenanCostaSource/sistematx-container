# IMAGEM
FROM tomcat:8.5

MAINTAINER Bruno Correia <brunogomescorreia@gmail.com>

# INSTALL PACKETS
RUN apt-get update -y && \ 
	apt-get install gettext-base openjdk-8-jdk -y

COPY ./files/context.xml /usr/local/tomcat/webapps/manager/META-INF/

COPY ./files/context.xml /usr/local/tomcat/webapps/host-manager/META-INF/

ADD ./files/esapi.tar.gz /root/

COPY ./files/*-template /tmp/

COPY ./scripts/orgSistematx /usr/local/bin/
