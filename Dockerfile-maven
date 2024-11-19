# Use the specified base image
FROM cepgbaseacr.azurecr.io/docker.io/openjdk:17-slim

# Set the working directory
WORKDIR /app

# Copy Maven build artifact (JAR file) to the container
COPY target/*.jar app.jar

# Expose the port your application will run on (if needed, e.g., 8080)
EXPOSE 8080

# Define the default command to run your application
ENTRYPOINT ["java", "-jar", "/app.jar"]
