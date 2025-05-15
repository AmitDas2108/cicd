# Use NGINX as base image
FROM nginx:alpine

# Copy website files into nginx directory
COPY . /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# No CMD needed; nginx image already has one
