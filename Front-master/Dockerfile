# Use the official Node.js 14 image as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install the dependencies in the container
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Build the Angular application
RUN npm run build

# Expose the port the app runs on
EXPOSE 4202

# Command to start the Angular application
CMD ["npm", "start"]