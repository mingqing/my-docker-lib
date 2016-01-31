# Version: 0.0.1

FROM centos:6

MAINTAINER MingQing Lee "mingqing@henji.org"

ADD nginx/nginx.repo /etc/yum.repos.d/nginx.repo

RUN yum install -y nginx.x86_64
RUN mkdir -p /usr/share/nginx/html

ADD nginx/nginx.conf /etc/nginx/nginx.conf
ADD nginx/default.conf /etc/nginx/conf.d/default.conf
ADD nginx/index.html /usr/share/nginx/html/index.html

EXPOSE 80

#CMD ["nginx"]
