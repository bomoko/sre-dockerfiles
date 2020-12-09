FROM alpine:latest

RUN apk update && apk --no-cache add git curl make python3 python3-dev gcc libc-dev libffi-dev py3-pip openssl-dev && pip3 --no-cache-dir install --upgrade pip && pip3 --no-cache-dir install docker-compose==1.24.1 && rm -f /var/cache/apk/*  && rm -rf /root/.cache

RUN curl -L "https://github.com/amazeeio/lagoon-cli/releases/download/0.10.0/lagoon-cli-0.10.0-linux-amd64" -o /usr/local/bin/lagoon && chmod +x /usr/local/bin/lagoon
