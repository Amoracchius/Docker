FROM ubuntu:18.04

RUN apt-get -y update
RUN apt-get -y install apache2

RUN echo 'Static page for devops team from container!' > /var/www/html/index.html

COPY . .

CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
