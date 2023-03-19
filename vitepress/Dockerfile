FROM node:16-alpine3.14

WORKDIR /app

COPY . .

RUN npm install
#RUN npm run build vitepress



EXPOSE 5173

CMD ["npm", "run",  "config.js\index.md"]