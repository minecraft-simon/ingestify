# Use the Quarkus base image
FROM quay.io/quarkus/ubi-quarkus-native-image:22.0.0-java11

# Set the working directory
WORKDIR /work/

# Copy your Quarkus application jar file into the container
COPY target/*-runner /work/application

# Set the execution permissions
RUN chmod 775 /work

# Specify the command to run your Quarkus application
CMD ["./application", "-Dquarkus.http.host=0.0.0.0"]