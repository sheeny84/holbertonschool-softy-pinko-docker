# Use the official latest Ubuntu image as the base
FROM ubuntu:latest

# Run commands to update software
RUN apt-get update && apt-get upgrade -y

# Install python3, python3-pip and flask
RUN apt-get install python3 -y
RUN apt-get install python3-pip -y
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED
RUN pip3 install Flask

# Set working directoty 
WORKDIR /app

# Copy python file to image
COPY api.py /app

# Expose port 5252
EXPOSE 5252

# Define the command to run flask when the container starts
CMD ["python3", "api.py"]