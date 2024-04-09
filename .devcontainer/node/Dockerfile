FROM node:20-alpine

WORKDIR /workspace
RUN apk update && apk upgrade \
    && apk add bash tzdata jq git \
    && ln -s /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
    && git config --global --add safe.directory "/workspace"
ENV SHELL=bash
ENTRYPOINT [ "/bin/bash" ]