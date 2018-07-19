# hello-world
FROM ubuntu
MAINTAINER  your_name  <user@domain.tld>
RUN apt-get update
RUN apt-get -y install apache2
RUN echo "Hi There !!!!! This is Sample Service03 used by devops for testing" > /var/www/html/index.html
EXPOSE 80
CMD /usr/sbin/apache2ctl -D FOREGROUND
