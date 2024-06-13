# Use the official Node.js image
FROM node:14

# Create and change to the app directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy app source code
COPY . .

# Expose the app port
EXPOSE 3001

# Run the app
CMD ["npm", "start"]