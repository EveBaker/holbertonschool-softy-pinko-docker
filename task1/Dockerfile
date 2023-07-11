# Use the latest Ubuntu base image
FROM ubuntu:latest

# Updates atp repo
Run apt-get update && apt-get install -y python3 python3-pip

# Install Flask using pip3
RUN pip3 install Flask

# Set the working directory to /app
WORKDIR /app

#Copy Python file to the working directory in the Docker image
COPY api.py /app

# inform Docker that the container listens
EXPOSE 5252

# Set the command to run on the Flask Server
CMD ["python3", "api.py"]
