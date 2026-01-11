# 1. Use Node.js image
FROM node:18-alpine

# 2. Set working directory inside container
WORKDIR /app

# 3. Copy package files
COPY package*.json ./

# 4. Install dependencies
RUN npm install

# 5. Copy rest of the frontend code
COPY . .

# 6. Expose React port
EXPOSE 3000

# 7. Start the app
CMD ["npm", "start"]

