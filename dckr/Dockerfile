FROM ubuntu:24.04
WORKDIR /home/vinayak
RUN apt update
WORKDIR /opt
RUN apt install wget -y
RUN wget https://dlcdn.apache.org/tomcat/tomcat-11/v11.0.18/bin/apache-tomcat-11.0.18.tar.gz
RUN tar -xvf apache-tomcat-11.0.18.tar.gz | mkdir tomcat11
WORKDIR /home/vinayak
COPY python_scripts/memory.py .
