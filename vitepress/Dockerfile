FROM node:16-alpine3.14

WORKDIR /app

COPY . .

RUN npm install
#RUN npm run vitepress

#RUN npm run build
#RUN apt-get update && apt-get upgrade -y &&  apt-get install -y nodejs  npm 


EXPOSE 5173

CMD ["npm run vitepress",  "config.js/index.md"]