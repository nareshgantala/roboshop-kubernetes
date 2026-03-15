FROM nginx:stable-alpine3.23-perl
RUN rm -rf /usr/share/nginx/html/* 
ADD https://roboshop-artifacts.s3.amazonaws.com/frontend.zip /usr/share/nginx/html
COPY . /etc/nginx/default.d/roboshop.conf 
