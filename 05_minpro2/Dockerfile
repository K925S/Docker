FROM quay.io/centos/centos:stream9

RUN yum -y install httpd php && yum clean all

VOLUME /var/www/html /var/log/httpd

# ADD src.tar /var/www/html
COPY index.html /var/www/html
COPY info.php /var/www/html
COPY entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh

EXPOSE 80

ENTRYPOINT ["/entrypoint.sh"]