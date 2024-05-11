FROM alpine
SHELL["/bin/bash", "-c"]
RUN apk update && add --update --no-cache \
bash curl wget busybox-extras netcat-openbsd python3 py3-pip
RUN pip --no-cache-dir install --upgrade awscli
RUN apk --purge -v del py-pip
CMD tail -f /dev/null
