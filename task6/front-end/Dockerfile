# Use the official latest nginx image as the base
FROM nginx:latest

# Copy python file to image
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy nginx config file
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf