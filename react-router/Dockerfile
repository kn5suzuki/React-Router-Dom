# Start with the Ubuntu base image
FROM ubuntu:latest

# Avoid prompts with apt-get
ENV DEBIAN_FRONTEND=noninteractive

# Update and install required packages
RUN apt-get update && apt-get install -y \
    curl \
    gnupg2 \
    nginx

# Add Node.js official LTS repository
RUN curl -fsSL https://deb.nodesource.com/setup_20.x | bash -

# Install Node.js
RUN apt-get install -y nodejs

WORKDIR /app
COPY package.json .

# Start and enable nginx. Since Docker containers run in the foreground, 
# the CMD instruction is used to start nginx in non-daemon mode.
CMD ["nginx", "-g", "daemon off;"]

# Expose port 80 for nginx
EXPOSE 80
