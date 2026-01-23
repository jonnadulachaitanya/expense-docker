FROM node:20.20.0-alpine3.23
EXPOSE 8080
ENV DB_HOST="mysql"
RUN mkdir /opt/server
WORKDIR /opt/server
COPY /code/package.json .
COPY /code/*.js .
RUN npm install
#We can start the app based on package.json, our code has no start command so we need to using index.js as we entioned it in main.
CMD ["node", "index.js"]

