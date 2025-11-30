FROM node:18-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./

# Install production dependencies only
RUN npm install --only=production

# Copy source code
COPY . .

EXPOSE 3003

# Use node directly to run the server
CMD ["node", "server.js"]
