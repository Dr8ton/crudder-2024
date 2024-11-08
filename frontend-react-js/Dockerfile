FROM node:16.18

# Set environment variables
ENV PORT=3000

# Set working directory
WORKDIR /frontend-react-js

# Copy only package.json and package-lock.json first for dependency installation
COPY package*.json ./
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the specified port
EXPOSE ${PORT}

# Default command to run the application
CMD ["npm", "start"]
