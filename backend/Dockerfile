FROM node:20
EXPOSE 8080
ENV DB_HOST="mysql"
RUN mkdir /tmp/server
WORKDIR /tmp/server
COPY /code/package.json .
COPY /code/*.js .
RUN npm install
#We can start the app based on package.json, our code has no start command so we need to using index.js as we entioned it in main.
CMD ["node", "index.js"]

