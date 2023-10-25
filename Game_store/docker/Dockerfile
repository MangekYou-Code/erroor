# Use a base image with OpenJDK 17 (or the version you have installed)
FROM adoptopenjdk:17-jre-hotspot

# Expose the port your application listens on
EXPOSE 8070

# Set the environment variable for the application home directory
ENV APP_HOME /usr/src/app

# Copy your Spring Boot JAR file into the container
COPY target/Game_store-0.0.1-SNAPSHOT.jar $APP_HOME/app.jar

# Set the working directory
WORKDIR $APP_HOME

# Define the entry point to run your application
ENTRYPOINT exec java -jar app.jar
