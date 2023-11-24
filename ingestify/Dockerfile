# Use a minimal base image
FROM ubuntu:latest

# Create a directory in the container to hold your files
WORKDIR /application

# Copy the native executable into the container
COPY build/quarkus-app /application

# Set the execution permissions
RUN chmod 775 /application

# Specify the command to run your Quarkus application
CMD ["/application", "-Dquarkus.http.host=0.0.0.0"]