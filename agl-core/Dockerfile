FROM node:20-alpine

WORKDIR /app/agl-core

EXPOSE 3000

RUN npm i -g nodemon

CMD ["nodemon", "--watch", ".", "--watch", "../agl-custom-middleware", "--ext", "js,json", "server.js"]
