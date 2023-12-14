# Use a Node.js base image
FROM node:18.12-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all files from the current directory to the working directory
COPY . .

# Build the React app
RUN npm run build

# Expose the port your React app runs on
EXPOSE 5173

# Set the startup command
CMD ["npm", "run", "dev"]
