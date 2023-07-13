FROM ubuntu:focal

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y apache2 git
RUN git clone https://github.com/LOFL404/static-web-template.git
RUN cp -r static-web-template/* /var/www/html


# Apache2 실행
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]

# 컨테이너의 80번 포트 열기
EXPOSE 80
