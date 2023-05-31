FROM ubuntu:22.04

RUN apt-get update && apt-get install -y nginx && apt-get clean
WORKDIR /webtest
VOLUME /test
COPY . /test
RUN cp /test/index.html /usr/share/nginx/html/index.html && cp /test/nginx.conf /etc/nginx/nginx.conf
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80