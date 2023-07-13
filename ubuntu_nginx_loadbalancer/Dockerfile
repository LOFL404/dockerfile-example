FROM ubuntu:focal
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update
RUN apt-get install -y nginx
COPY sites-available/loadbalancer /etc/nginx/sites-available/default
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80