# Node image
FROM node:latest
# Create code directory
RUN mkdir /code
# Set working directory
WORKDIR /code
# Install Truffle
RUN npm install -g truffle
# Fix to prevent error:0308010C:digital envelope routines::unsupported
ENV NODE_OPTIONS=--openssl-legacy-provider
# Install net-tools
RUN apt-get update && apt-get install -y iputils-ping
# Note: This container needs to be started with a command that prevent immediate termination 

