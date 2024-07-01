# Use this version of ubuntu for base image
FROM ubuntu:22.04

# Update package lists and install packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask

# Setting working directory and copying the Python file to Docker image
WORKDIR /app
COPY api.py /app/api.py

# Commands to run
CMD ["python3", "/app/api.py"]

# To Build: docker build -f ./Dockerfile -t softy-pinko:task1 .
# To Run: docker run -p 5252:5252 -it --rm --name softy-pinko-task1 softy-pinko:task1