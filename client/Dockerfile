FROM node:lts-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY .. .
RUN npm run build
RUN npm install -g serve
EXPOSE 3000
RUN npm install -g serve

CMD ["npm", "start"]

                