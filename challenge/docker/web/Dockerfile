# Version: 0.0.1
FROM centos:latest

LABEL maintainer=“gerard@solvinity.com”

RUN yum install epel-release -y
RUN yum update -y
RUN yum install nginx -y
RUN yum clean all

COPY nginx.conf /etc/nginx/
COPY index.html /usr/share/nginx/html

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]
