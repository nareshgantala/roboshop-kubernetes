FROM nginx:stable-alpine3.23-perl
RUN rm -rf /usr/share/nginx/html/* 
WORKDIR /app
ADD https://roboshop-artifacts.s3.amazonaws.com/frontend.zip /app
RUN cd /usr/share/nginx/html 
RUN unzip /app/frontend.zip
COPY . /etc/nginx/default.d/roboshop.conf 
