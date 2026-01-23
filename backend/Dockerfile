FROM node:20
EXPOSE 8080
ENV DB_HOST="mysql"
RUN mkdir /tmp/server
WORKDIR /tmp/server
COPY /code/package.json .
COPY /code/*.js .
RUN npm install
CMD ["node", "index.js"]

