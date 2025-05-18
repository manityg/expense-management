# Use an official Node.js image
FROM node:18

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json first to leverage Docker cache
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all other source files
COPY . .

# Expose the port that React runs on in dev mode
EXPOSE 3000

# Start the development server
CMD ["npm", "start"]
