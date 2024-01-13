FROM ubuntu:latest

ARG vdir=Fokeman 
WORKDIR /WeatherApp

RUN apt install -y nodejs
COPY $vdir/node_modules ./WeatherApp

RUN apt install npm 
COPY $vdir/public ./WeatherApp
COPY $vdir/views ./WeatherApp

RUN npm install -g express 
COPY $vdir/package.json .

COPY $vdir/package-lock.json .
COPY $vdir/server.js .
RUN npm install ejs 

EXPOSE 8000

CMD ["npm" "start"]
