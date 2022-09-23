FROM node:16
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies

COPY ./udagram-api-feed/package*.json ./

# COPY package-lock.json /usr/src/app

RUN ls

RUN npm ci 
# Bundle app source
COPY ./udagram-api-feed .
EXPOSE 8080
CMD [ "npm", "run", "prod" ]
