FROM alpine:3.18

RUN apk -i update && apk -i add nginx
WORKDIR /webtest2
VOLUME /test2
COPY . /test2
RUN cp /test2/index.html /var/lib/nginx/html/index.html && cp /test2/nginx.conf /etc/nginx/nginx.conf
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 81