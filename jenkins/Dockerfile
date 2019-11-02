FROM jenkins/jenkins
USER root
RUN curl -o /tmp/filebeat_1.0.1_amd64.deb https://download.elastic.co/beats/filebeat/filebeat_1.0.1_amd64.deb && dpkg -i /tmp/filebeat_1.0.1_amd64.deb &&  apt-get install
COPY ./filebeat.yml  /etc/filebeat/filebeat.yml
RUN apt-get update
RUN apt-get install python-pip -y
