FROM node:20

WORKDIR /myapp

# Copy only package.json first (better caching)
COPY package*.json ./

# Install dependencies
RUN npm install

# Now copy the rest of the project files
COPY . .

# Expose React default port
EXPOSE 3000

# Run the development server
CMD ["npm", "start"]
