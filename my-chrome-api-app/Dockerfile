# Use official Node.js image as a base
FROM node:16-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json for dependency installation
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the app files into the container
COPY . .

# Expose port 3000 (default for React apps)
EXPOSE 3000

# Start the React app when the container runs
CMD ["npm", "start"]
