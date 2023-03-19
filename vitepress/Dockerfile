FROM node:16-alpine3.14

WORKDIR /app

COPY . .

RUN npm install

RUN npm run build

EXPOSE 4173

CMD ["npm", "run", "docs:preview"]
