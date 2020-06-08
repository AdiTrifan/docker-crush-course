FROM openjdk:8-jdk-alpine
EXPOSE 8080
ARG DEPENDENCY=target/dependency
COPY ${DEPENDENCY}/BOOT-INF/lib /app.lib
COPY ${DEPENDENC}/META-INF /app/META-INF
COPY ${DEPENDENCY}/BOOT-INF/classes /app
#ADD target/hello-world-rest-api.jar hello-world-rest-api.jar
#ADD target/*.jar app.jar
#ENTRYPOINT ["sh", "-c", "java -jar /app.jar"]
ENTRYPOINT ["java", "-cp", "app:app/lib/*", "com.in28minutes.rest.webservices.restfulwebservices.RestfulWebServicesApplication"]

