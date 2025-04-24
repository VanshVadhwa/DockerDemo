# Use official Node image
FROM node:18

# Set working directory
WORKDIR /App

# Copy only package.json and lock file first (for caching)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the source code
COPY . .

# Expose the port Vite runs on
EXPOSE 3000

# Start the Vite dev server
CMD ["npm", "run", "dev"]
