FROM node:18.19.0-alpine as build

COPY ./ /frontend
WORKDIR /frontend
RUN apk update & npm install
RUN npm run build

FROM nginx:alpine
COPY --from=build frontend/dist /var/www
COPY ./multiStage/default.conf /etc/nginx/conf.d/

WORKDIR /usr/share/nginx/html
CMD ["nginx", "-g", "daemon off;"]