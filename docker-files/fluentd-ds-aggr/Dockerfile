FROM fluent/fluentd:v0.12
USER root

RUN apk add --update --virtual .build-deps \
        sudo build-base ruby-dev
 # cutomize following instruction as you wish
RUN  fluent-gem install fluent-plugin-elasticsearch
COPY ./config/fluent.conf ./fluentd/etc/
EXPOSE 24224