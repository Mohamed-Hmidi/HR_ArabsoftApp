# Use the official OpenJDK image as a base
FROM openjdk:17-jdk-alpine

# Set the working directory in the container
WORKDIR /app

# Copy the executable JAR file from the local machine to the container
COPY target/Authpfe-0.0.1-SNAPSHOT.jar app.jar

# Expose the port on which the Spring Boot app will run
EXPOSE 8090

# Run the JAR file
ENTRYPOINT ["java", "-jar", "app.jar"]
