FROM centos:centos7
MAINTAINER jgasper@unicon.net

RUN yum -y update \
    && yum -y install httpd \
    && yum -y clean all

COPY httpd-foreground /usr/local/bin/

EXPOSE 80

CMD ["httpd-foreground"]