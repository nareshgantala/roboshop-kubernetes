FROM nginx:stable-alpine3.23-perl
RUN rm -rf /usr/share/nginx/html/* 
ADD https://roboshop-artifacts.s3.amazonaws.com/frontend.zip /usr/share/nginx/html
WORKDIR /usr/share/nginx/html
RUN unzip frontend.zip
COPY roboshop.conf /etc/nginx/default.d
