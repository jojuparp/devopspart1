FROM openjdk:latest

WORKDIR /usr/src/myapp
EXPOSE 8080
COPY . /usr/src/myapp
RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]