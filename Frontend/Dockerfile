FROM node:18-alpine

WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy application code
COPY . .

# Expose port for Vite dev server
EXPOSE 5173

# Start development server with explicit host binding
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]
