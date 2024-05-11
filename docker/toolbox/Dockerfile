FROM alpine
RUN apk update && add --update --no-cache \
    curl wget busybox-extras netcat-openbsd python3 py3-pip
RUN pip --no-cache-dir install --upgrade awscli
RUN apk --purge -v del py-pip
CMD tail -f /dev/null
