#Rocky_Apache

FROM rockylinux:9.3

LABEL maintainer=naruto@naruto.com

RUN dnf -y install epel-release && \
    dnf makecache && \
    dnf -y install httpd && \
    dnf clean all

COPY index.html /var/www/html/index.html

EXPOSE 80

CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]

