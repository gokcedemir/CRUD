FROM node:16-buster AS publish

COPY . ./build
WORKDIR build

RUN npm install
RUN npm install typescript@4.0.2 -g 
 
RUN npm run

FROM nginxinc/nginx-unprivileged:latest AS start 
EXPOSE 80 
WORKDIR app 
 
ENV TZ=Europe/Istanbul 
COPY default.conf /etc/nginx/conf.d/default.conf