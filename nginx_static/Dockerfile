FROM nginx
COPY nginx.conf /etc/nginx/nginx.conf
COPY lab.jpeg /www/data/images/lab.jpeg
COPY dd-config.json /etc/dd-config.json

RUN apt-get update && apt-get install -y wget curl
COPY setup_dd.sh /setup_dd.sh
RUN /setup_dd.sh