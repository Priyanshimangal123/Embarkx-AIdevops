FROM eclipse-temurin:21-jdk
RUN mkdir /opt/app
COPY target/*.jar app.jar
CMD ["java", "-jar", "app.jar"]
