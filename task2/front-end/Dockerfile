#  Instead of using ubuntu use nginx
FROM nginx:latest

# Copy front-end to Docker image
ADD softy-pinko-front-end /var/www/html/softy-pinko-front-end
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
