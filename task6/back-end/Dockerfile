# Use this version of ubuntu for base image
FROM ubuntu:22.04

# Update package lists and install packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask flask-cors

# Setting working directory and copying the Python file to Docker image
WORKDIR /app
COPY api.py /app/api.py

# Commands to run
CMD ["python3", "/app/api.py"]

# To Build: docker build -f ./back-end/Dockerfile -t softy-pinko-back-end:task3 ./back-end
# To Run: docker run -p 5252:5252 -it --rm --name softy-pinko-back-end-task3 softy-pinko-back-end:task3