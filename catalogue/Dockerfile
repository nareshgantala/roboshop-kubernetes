FROM node:25-alpine3.22
WORKDIR /app
RUN adduser -D roboshop
ADD https://roboshop-artifacts.s3.amazonaws.com/catalogue.zip /app/
RUN unzip catalogue.zip
RUN npm install
ENV MONGO_URL="mongodb://<MONGODB-SERVER-IPADDRESS>:27017/catalogue"
CMD ["node", "server,js"]