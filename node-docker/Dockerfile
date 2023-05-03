FROM node:18-alpine
#env could also be production
ENV NODE_ENV=staging 

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm install --staging

COPY . .

CMD ["node", "server.js"]
