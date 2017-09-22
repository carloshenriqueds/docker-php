FROM nimmis/apache-php5

MAINTAINER Carlos Henrique <carlossantosdm@gmail.com>

RUN echo "nameserver 8.8.8.8" | tee /etc/resolv.conf

# Copy this repo into place.
ADD . /var/www/html/$PROJECT_FOLDER

EXPOSE 80
EXPOSE 443

CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]