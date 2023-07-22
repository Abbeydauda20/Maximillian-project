# Use the official Node.js image as the base image
FROM node:14

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json (if available)
COPY . /app

# Install Node.js dependencies 
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Expose the port on which your Node.js application is listening
EXPOSE 80

# Command to start your Node.js application
CMD ["node", "server.js"]
