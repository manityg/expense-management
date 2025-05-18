# Use official Node.js LTS image
FROM node:18

# Set working directory inside the container
WORKDIR /app

# Copy package files first to install dependencies
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose the port your app runs on
EXPOSE 5000

# Start the application
CMD ["npm", "run", "dev"]
