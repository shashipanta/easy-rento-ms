# Use an official OpenJDK runtime as a parent image
FROM openjdk:17-jdk-slim

# Set working directory inside container
WORKDIR /app

# Copy the jar built by Maven/Gradle into the container
COPY target/*.jar app.jar

# Run the jar
ENTRYPOINT ["java","-jar","app.jar"]
