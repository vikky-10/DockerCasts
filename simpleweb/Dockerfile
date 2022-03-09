# Specify a base image
FROM node:alpine

WORKDIR /usr/app

# Install some depenendencies
# add package.json because package.json our 
# container not add package.json inside the container
# and without package.json application not work

COPY ./package.json ./    
RUN npm install
COPY ./ ./

# Default command
CMD ["npm", "start"]