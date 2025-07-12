# Use official node js image
From node:18

# Set working dir
WORKDIR /app

# Copy dependency file and install
COPY package*.json ./
RUN npm install

#Copy rest of the app
COPY . .

# Start the app
CMD ["node", "app.js"]