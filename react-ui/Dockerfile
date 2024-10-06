FROM node:20-alpine as build
WORKDIR /app
ENV PATH /app/node_modules/.bin:$PATH
COPY ./package*.json /app/
RUN npm install
COPY . /app
RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]