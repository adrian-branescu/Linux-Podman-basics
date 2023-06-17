FROM nginx:mainline-alpine

RUN rm /etc/nginx/conf.d/*

ADD hello.conf /etc/nginx/conf.d/

ADD index.html /usr/share/nginx/html/

RUN mkdir /usr/share/nginx/html/images/

ADD images/image.png /usr/share/nginx/html/images/
