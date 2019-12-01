FROM jenkins/jenkins
USER root
RUN curl -o /tmp/filebeat_7.4.2_amd64.deb https://artifacts.elastic.co/downloads/beats/filebeat/filebeat-7.4.2-amd64.deb && dpkg -i /tmp/filebeat_7.4.2_amd64.deb && apt-get install
COPY ./filebeat.yml  /etc/filebeat/filebeat.yml
RUN apt update -y
RUN apt install -y python-pip
