## Nginx Dockerfile


### Base Docker Image

* [ubuntu:14.04.2](https://registry.hub.docker.com/_/ubuntu/)

### Usage

    docker run -d -p 80:80 -p 443:443 pbecker/nginx

#### Volumes

    Volume: <sites-enabled-dir>:/etc/nginx/conf.d
    Volume: <certs-dir>:/etc/nginx/certs
    Volume: <log-dir>:/var/log/nginx
    Volume: <html-dir>:/var/www/html

Open `http://<host>` to see the welcome page.
