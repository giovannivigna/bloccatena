# Node image
FROM node:latest
# Create app directory
RUN mkdir /app
# Set working directory
WORKDIR /app
# Install Truffle
RUN npm install -g ganache-cli
# Fix to prevent error:0308010C:digital envelope routines::unsupported
ENV NODE_OPTIONS=--openssl-legacy-provider
# Set the default command for the image
CMD ["ganache-cli", "-h", "0.0.0.0"]