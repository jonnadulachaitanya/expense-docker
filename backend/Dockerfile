FROM node:20
EXPOSE 8080
END DB_HOST="mysql"
RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npn install
CMD ["node", "index.js"]
