FROM node:carbon

# Create app directory
RUN mkdir -p /usr/src/grpc-client
WORKDIR /usr/src/grpc-client

# Install app dependencies
COPY package.json /usr/src/grpc-client
RUN npm install

# Bundle app source
COPY . /usr/src/grpc-client

EXPOSE 3000

CMD [ "node", "client/index.js" ]