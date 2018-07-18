FROM centos:6
RUN set -ex \
    && yum update -y \
    && yum install nginx -y

RUN echo 'hoge' > /usr/share/nginx/html/index.html

CMD /usr/sbin/nginx -g "daemon off;" -c /etc/nginx/nginx.conf
