# FROM node:lts-alpine
# ENV NODE_ENV=development
# WORKDIR /usr/src/app
# COPY ./social_connect_app_frontend/package.json ./
# COPY ./social_connect_app_frontend/package-lock.json ./
# RUN  npm install react-scripts --legacy-peer-deps
# RUN mkdir ./node_modules/.cache && chmod -R 777 ./node_modules/.cache
# # RUN  npm install -g npm@9.1.2
# COPY ./social_connect_app_frontend /usr/src/app
# EXPOSE 3000
# USER node
# CMD ["npm","start"]

FROM node:lts-alpine
ENV NODE_ENV=development
WORKDIR /usr/src/cache
COPY ./social_connect_app_frontend/package.json ./
COPY ./social_connect_app_frontend/package-lock.json ./
RUN  npm install react-scripts --legacy-peer-deps
# RUN  npm install -g npm@9.1.2
WORKDIR /usr/src/app
COPY ./social_connect_app_frontend /usr/src/app
EXPOSE 3000
# USER node
# CMD ["npm","start"]

