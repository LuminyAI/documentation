# Use an official Nginx image as a base
FROM nginx:alpine

# Copy the built Docusaurus files to the nginx HTML directory
COPY build /usr/share/nginx/html

# Copy custom Nginx configuration
COPY nginx.conf /etc/nginx/nginx.conf

# Expose port 80
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
