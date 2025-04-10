# Use a lightweight web server
FROM nginx:alpine

# Remove default nginx index page
RUN rm -rf /usr/share/nginx/html/*

# Copy your web files into nginx html directory
COPY . /usr/share/nginx/html

# Expose port 80
EXPOSE 80
