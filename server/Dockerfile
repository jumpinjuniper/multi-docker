# Use an existing docker image as a base
FROM node:14.14.0-alpine
WORKDIR /usr/app

# Download and install a dependency
COPY ./package.json ./
RUN npm install

# Copy existing file structure to container
COPY ./ ./

# Tell the image what to do when it starts as a container
CMD ["npm", "run", "start"]