FROM ubuntu:20.10

USER root

RUN apt-get update \
    && apt-get install -y nginx \
    && rm -rf /var/www/html/index.nginx-debian.html

COPY index.html /var/www/html/index.html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
