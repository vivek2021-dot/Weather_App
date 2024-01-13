FROM ubuntu:latest

ARG vdir=Fokeman 
WORKDIR /WeatherApp

RUN apt update && \ apt install -y nodejs npm

COPY $vdir/node_modules ./WeatherApp/node_modules
COPY $vdir/public ./WeatherApp/public
COPY $vdir/views ./WeatherApp/views

RUN npm install -g express
COPY $vdir/package.json .
COPY $vdir/package-lock.json .
COPY $vdir/server.js .

RUN npm install ejs 

EXPOSE 8000

CMD ["npm", "start"]
