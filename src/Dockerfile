# Step 1: Build the React app
FROM node:16

# Set the working directory inside the container
WORKDIR /app

# Copy the package.json and package-lock.json
COPY package*.json ./

# Install the app dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port for the React dev server
EXPOSE 3000

# Start the React dev server
CMD ["npm", "start"]