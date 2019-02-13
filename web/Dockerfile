# this is my first docker file to create my apache
FROM centos:7
MAINTAINER anusha.gunnam0411@gmail.com
# we need to update yum it is recommeded in centos and required in redhat and ubuntu etc
RUN yum -y update
RUN yum -y install httpd
ADD code /var/www/html
#ports we are running--meta data
EXPOSE 80
#environment variables declaration---Meta data
ENV BACKENDLB=test
CMD ["apachectl", "-D", "FOREGROUND"]
