# Use the official OpenJDK 17 image as the base image
FROM openjdk:17

# Set the working directory inside the container
WORKDIR /app

# Copy your Kotlin/Java application JAR file into the container
COPY . /app

# Command to run your application when the container starts
CMD ["java", "-jar", "quarkus-run.jar"]
