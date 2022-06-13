# Node image
FROM node:latest
# Create code directory
RUN mkdir /code
# Set working directory
WORKDIR /code
# Install Truffle
RUN npm install -g truffle
# Install net-tools
RUN apt-get update && apt-get install -y iputils-ping vim
# Note: This container needs to be started with a command that prevent immediate termination 

