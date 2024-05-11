FROM alpine
RUN apt-get update
RUN apk add --no-cache curl wget busybox-extras netcat-openbsd python3 py-pip python3-pip python3-setuptools
RUN pip3 --no-cache-dir install --upgrade awscli
RUN apk --purge -v del py-pip
CMD tail -f /dev/null
