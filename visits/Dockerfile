# Specify a base image
FROM node:alpine

# Set the working directory inside the container
WORKDIR /usr/app

# Copy package.json and package-lock.json (if exists) to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . /usr/app/app.js

# Default command
CMD ["npm", "start"]
