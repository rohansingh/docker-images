FROM onescience/alpine
MAINTAINER Rohan Singh "rohan@washington.edu"

RUN apk-install nginx && mkdir /tmp/nginx

EXPOSE 80

CMD ["nginx", "-g", "daemon off; error_log stderr info;"]
