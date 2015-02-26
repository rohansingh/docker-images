FROM gliderlabs/alpine:3.1
MAINTAINER Rohan Singh "rohan@washington.edu"

RUN apk-install nginx && mkdir /tmp/nginx

ENTRYPOINT ["nginx"]
CMD ["-g", "daemon off;"]
