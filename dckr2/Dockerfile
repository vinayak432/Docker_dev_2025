FROM ubuntu:24.04
ARG FIRST_ARG
ARG SECOND_ARG
ENV FIRST_ARG=${FIRST_ARG}
ENV SECOND_ARG=${SECOND_ARG}
WORKDIR /home/vinayak/
RUN apt update
RUN apt install python3 -y
COPY shellscript_devops2025 ./shellscript_devops2025
RUN chmod u+x shellscript_devops2025/*.sh
COPY python_scripts ./python_scripts
RUN chmod u+x python_scripts/*.py
