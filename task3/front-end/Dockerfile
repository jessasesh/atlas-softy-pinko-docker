#  Instead of using ubuntu use nginx
FROM nginx:latest

# Copy front-end to Docker image
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# To Build: docker build -f ./front-end/Dockerfile -t softy-pinko-front-end:task2 ./front-end
# To Run: docker run -p 9000:9000 -it --rm --name softy-pinko-front-end-task2 softy-pinko-front-end:task2