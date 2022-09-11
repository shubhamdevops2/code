FROM node
LABEL maintainer="Shubham Kawale <shubham.devops.2@gmail.com>"

RUN apt-get update && apt-get -y upgrade

WORKDIR /app

#COPY ["package.json", "package-lock.json*", "./"]

ADD "*.tgz" "$PWD/"
RUN tar -xvfz *.tgz
WORKDIR /app/package

RUN npm install

CMD ["node","app.js"]
