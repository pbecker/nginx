## Nginx Dockerfile

This Docker Image can be used for a nginx proxy.

### Base Docker Image

* [ubuntu:14.04.2](https://registry.hub.docker.com/_/ubuntu/)

### Nginx PPA

* [Nginx](http://wiki.nginx.org/Install)

### Usage

    docker run -d -p 80:80 -p 443:443 pbecker/nginx

### Mountable volumes

    Volume: <sites-enabled-dir>:/etc/nginx/sites-enabled
    Volume: <additional-config-dir>:/etc/nginx/conf.d
    Volume: <certs-dir>:/etc/nginx/certs
    Volume: <log-dir>:/var/log/nginx
    Volume: <html-dir>:/var/www/html
