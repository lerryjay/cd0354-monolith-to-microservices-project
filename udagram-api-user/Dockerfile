FROM node:13
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies

COPY ./udagram-api-user/package*.json ./
RUN npm ci 
# Bundle app source
COPY ./udagram-api-user .
EXPOSE 8080
CMD [ "npm", "run", "prod" ]
