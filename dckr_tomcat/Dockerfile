FROM ubuntu:24.04
MAINTAINER Vinayak
WORKDIR /opt
RUN apt update && \ 
    apt install default-jdk -y
ADD https://dlcdn.apache.org/tomcat/tomcat-11/v11.0.18/bin/apache-tomcat-11.0.18.tar.gz /opt
RUN tar -xzf apache-tomcat-11.0.18.tar.gz
RUN mv apache-tomcat-11.0.18 tomcat11

EXPOSE 8080

ENTRYPOINT ["/opt/tomcat11/bin/catalina.sh", "run"]
