# Use the official Node.js image
FROM node:14

# Create and change to the app directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install app dependencies
RUN npm install

# Install serve globally
RUN npm install -g serve

# Copy app source code
COPY . .

# Build the app
RUN npm run build

# Serve the app
EXPOSE 80
CMD ["serve", "-s", "build"]



