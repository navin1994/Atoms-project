# FROM node:18-alpine3.19

# WORKDIR /app

# # Copy package.json and package-lock.json
# COPY package.json package-lock.json ./

# # Install dependencies
# RUN npm install

# # Copy the rest of the application code
# COPY . .

# # Build the React application
# RUN npm run build

# # Command to serve the built app
# CMD ["npm", "run", "dev"]

FROM node:18-alpine3.19

WORKDIR /app

# Copy package.json and package-lock.json
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Build the React application
RUN npm run build

# Command to serve the built app
CMD ["npm", "run", "dev", "--", "--host"]
