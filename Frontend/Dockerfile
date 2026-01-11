# Step 1: Use Node.js
FROM node:18-alpine

# Step 2: Work inside /app
WORKDIR /app 

# Step 3: Copy dependency list
COPY package*.json ./

# Step 4: Install dependencies
RUN npm install

# Step 5: Copy all frontend code
COPY . .

# Step 6: React runs on port 8080
EXPOSE 8080

# Step 7: Start the app
CMD ["npm", "start"]
