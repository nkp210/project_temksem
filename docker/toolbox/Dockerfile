FROM alpine
RUN apk update && add --update --no-cache \
bash curl wget busybox-extras netcat-openbsd python3 py3-pip && ln -sf python3 /usr/bin/python
RUN python3 -m ensurepip && pip3 install --no-cache-dir --upgrade awscli
RUN apk --purge -v del py-pip
CMD tail -f /dev/null
