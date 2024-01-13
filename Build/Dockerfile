FROM ubuntu:latest

ARG vdir=Fokeman 
WORKDIR /WeatherApp

RUN apt-get update
RUN apt-get install -y nodejs npm 
COPY $vdir/node_modules ./WeatherApp/node_modules
COPY $vdir/public ./WeatherApp/public
COPY $vdir/views ./WeatherApp/views

RUN npm install -g express
COPY $vdir/package.json .
COPY $vdir/package-lock.json .
COPY $vdir/server.js .

RUN npm install ejs 

EXPOSE 3000

CMD ["npm", "start"]
