# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM eclipse-temurin:17-jre-alpine

# Define artifact path
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy the jar file into the container
COPY ${artifact} app.jar

# Set the entrypoint to run the jar
ENTRYPOINT ["java", "-jar", "app.jar"]

