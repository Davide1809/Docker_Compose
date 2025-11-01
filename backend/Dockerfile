# Step a: Use a Node.js base image
FROM node:18-alpine

# Step b: Set the working directory inside the container
WORKDIR /app

# Step c: Copy dependency files
COPY package*.json ./

# Step d: Install dependencies
RUN npm install --only=production

# Step e: Copy all the application files
COPY . .

# Step g: Expose the backend port (5000)
EXPOSE 5000

# Step h: Start the application
CMD ["npm", "start"]
