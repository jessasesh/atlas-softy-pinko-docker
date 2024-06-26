# Use this version of ubuntu for base image
FROM ubuntu:22.04

# Update package lists
RUN apt-get update
RUN apt-get upgrade -y

# Run commands
CMD ["echo", "Hello, World!"]

# To Build: docker build -f ./Dockerfile -t softy-pinko:task0 .
# To Run: docker run -it --rm --name softy-pinko-task0 softy-pinko:task0