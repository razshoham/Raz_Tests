# INSTRACTION PARAMETERS
FROM centos:latest
MAINTAINER razshoham
RUN yum -y install java-1.8.0-openjdk-devel
RUN yum -y install tomcat
ENV NAME whatever_for_tomcat
RUN mkdir /logs
CMD tomcat start && tail -f /logs/catalina.out
ADD *.war /usr/share/tomcat/webapps
