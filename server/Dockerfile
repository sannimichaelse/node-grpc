FROM node:carbon

# Create app directory
RUN mkdir -p /usr/src/grpc-server
WORKDIR /usr/src/grpc-server

# Install app dependencies
COPY package.json /usr/src/grpc-server
RUN npm install

# Bundle app source
COPY . /usr/src/grpc-server

CMD [ "node", "server/server.js" ]