# Use an official Node.js runtime as a parent image
FROM node:20.10.0

# Set the working directory inside the container
WORKDIR /Users/admin/Documents/shopify/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the application code into the container
COPY . .

# Expose the port on which your app will run
EXPOSE 3000

# Command to run your application
CMD ["npm", "start"]