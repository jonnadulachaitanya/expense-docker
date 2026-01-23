FROM node:20.20.0-alpine3.23
#We can save more memory by using alpine images
EXPOSE 8080
ENV DB_HOST="mysql"
RUN addgroup -S expense && adduser -S expense -G expense && \
  mkdir /opt/server && \
  chown -R expense:expense /opt/server
WORKDIR /opt/server
COPY /code/package.json .
COPY /code/*.js .
RUN npm install
USER expense
#We can start the app based on package.json, our code has no start command so we need to using index.js as we entioned it in main.
CMD ["node", "index.js"]

