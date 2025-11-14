# Node image suitable for development on any machine (x86 or ARM)
FROM node:20-bullseye

# Set working directory
WORKDIR /usr/src/app

# Copy package metadata first for caching
COPY ../package*.json ./

# Install dependencies
RUN npm install

# Install nodemon globally for auto-reload
RUN npm install -g nodemon

# Default command (overridden by docker-compose)
CMD ["npm", "start"]
