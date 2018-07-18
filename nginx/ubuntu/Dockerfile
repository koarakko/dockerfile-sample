FROM ubuntu:14.04.5
RUN set -ex \
    && apt-get update \
    && apt-get install nginx

RUN echo 'hoge' >  /usr/share/nginx/html/index.html

CMD /usr/sbin/nginx -g "daemon off;" -c /etc/nginx/nginx.conf
