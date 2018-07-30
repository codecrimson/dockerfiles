FROM node
FROM jenkins/jenkins:lts
ENV MONGODB_URI mongodb://MONGODB

USER root
RUN apt-get update && apt-get install -y gcc make libpng-dev
COPY --from=0 /usr/local  /usr/local

RUN npm install gulp-cli -g
USER jenkins
