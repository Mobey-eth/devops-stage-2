# Use an official Node.js runtime as the base image
FROM node:20-alpine


# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the frontend source code to the working directory
COPY . .

# Expose the port that the frontend application will run on
EXPOSE 5173

# Start the frontend application
CMD ["npm", "run", "dev"]