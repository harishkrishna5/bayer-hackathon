# Use an official Node.js image as the base image
FROM node:16

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to install dependencies first
COPY package*.json ./

# Install the app dependencies
RUN npm install

# Copy the rest of the application files to the container
COPY . .

# Expose the port that the app will run on
EXPOSE 3001

# Command to run the application
CMD ["node", "appointments-service.js"]
