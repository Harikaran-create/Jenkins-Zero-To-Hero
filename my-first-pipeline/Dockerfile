
# Use official Node.js 18 image as base
FROM node:18

# Set working directory inside the container
WORKDIR /app

# Copy only package files first (for caching npm install)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of your app files
COPY . .

# Expose the port your app runs on
EXPOSE 3000

# Command to run your Node app
CMD ["node", "app.js"]
