# For Java 8, try this
# FROM openjdk:8-jdk-alpine

# For Java 11, try this
FROM openjdk:8

# Refer to Maven build -> finalName
ARG JAR_FILE=target/mobile-banking.jar

# cd /opt/app
WORKDIR ../

# cp target/mobile-banking.jar /opt/app/app.jar
COPY ${JAR_FILE} app.jar

# java -jar /opt/app/app.jare
ENTRYPOINT ["java","-jar","app.jar"]