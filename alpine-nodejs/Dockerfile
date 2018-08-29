FROM docker:dind

RUN set -ex \
    && apk update \
    && apk upgrade \
    && apk add python build-base linux-headers

RUN set -ex \
    && wget http://nodejs.org/dist/v6.14.4/node-v6.14.4.tar.gz \
    && tar xf node-v6.14.4.tar.gz \
    && cd node-v6.14.4 \
    && ./configure --prefix=/ --without-snapshot --fully-static \
    && make -j2 \
    && make install \
    && cd .. \
    && rm -f node-v6.14.4.tar.gz \
    && rm -rf node-v6.14.4
