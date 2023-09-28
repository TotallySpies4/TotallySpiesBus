FROM node:18

# Use /usr/src/app as the workdir. The following instructions will be executed in this location
WORKDIR /usr/src/app

# Copy the the files require to install the dependencies
COPY ./package*.json ./

# Install the required dependencies
RUN npm install

# Copy the source code
COPY . .

# Run the test
CMD ["npm", "test"]