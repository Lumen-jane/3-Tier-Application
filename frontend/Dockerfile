# Use a lightweight Node.js image
FROM node:18-alpine3.18

# Set the working directory in the container
WORKDIR /application

# Copy package.json and package-lock.json (if available) to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose the port the app will run on (adjust as necessary)
EXPOSE 3000

# Command to start the application
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]
