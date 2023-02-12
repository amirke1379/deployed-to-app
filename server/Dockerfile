# Use an existing Node.js image as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy the package.json file to the container
COPY package*.json ./

# Install the required dependencies
RUN npm install

# Copy the rest of the app's files to the container
COPY . .

ENV USERNAME=postgres  
ENV PASSWORD=password
ENV HOST=0.0.0.0
ENV DBPORT=5432


# Specify the command to run when the container starts
CMD ["npm", "start"]
