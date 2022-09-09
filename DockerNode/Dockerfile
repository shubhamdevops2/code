FROM node
LABEL maintainer="Shubham Kawale <shubham.devops.2@gmail.com>"

#ARG SERVICE_NAME="myapp-0.0.7-SNAPSHOT"
RUN apt-get update && apt-get -y upgrade

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

#ADD "target/*.war" "$CATALINA_HOME/webapps/myapp.war"
RUN npm install

COPY . .

CMD ["node","app.js"]
