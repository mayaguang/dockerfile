FROM ubuntu:14.04
MAINTAINER mayaguang "358987589@qq.com"
RUN apt-get update
RUN  apt-get install -y apache2
ENV APACHE_RUN_USER wwww-data
ENV APACHE_RUN_GROUP wwww-data
ENV APATCHE_LOG_DIR /var/log/apatche2
ONBUILD ADD . /var/www/
EXPOSE 80
ENTRYPOINT ["/usr/sbin/apache2"]
CMD ["-D", "FOREGROUND"]

