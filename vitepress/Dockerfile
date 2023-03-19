FROM node:16-alpine3.14

COPY . .

RUN npm install
#RUN npm run vitepress

#RUN npm run build

EXPOSE 5000

CMD ["npm", "run", "docs:preview"]