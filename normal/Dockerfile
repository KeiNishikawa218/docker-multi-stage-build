FROM node:18.19.0-alpine

COPY ./ /frontend
WORKDIR /frontend
RUN apk update & npm install

CMD ["npm", "run", "dev"]
