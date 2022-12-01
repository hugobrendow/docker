FROM openjdk:17
COPY target/app.jar app.jar
EXPOSE 8099
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app.jar"]