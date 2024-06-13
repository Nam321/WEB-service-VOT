# Use the official Node.js image
FROM node:14

# Install http-server globally
RUN npm install -g http-server

# Create and change to the app directory
WORKDIR /app

# Copy public/index.html to the working directory
COPY public/index.html ./

# Expose port 80
EXPOSE 80

# Start the HTTP server and serve the index.html file
CMD ["http-server", ".", "-p", "80"]

#CMD ["serve", "-s", "build"]



# Copy package.json and package-lock.json
# COPY package*.json ./

# Install app dependencies
# RUN npm install

# Install serve globally
# RUN npm install -g serve

# Copy app source code
# COPY . .

# Build the app
# RUN npm run build

# Serve the app