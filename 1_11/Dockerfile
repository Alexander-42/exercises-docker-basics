FROM amazoncorretto:8-alpine3.21

WORKDIR /usr/src/app

COPY . .

RUN ./mvnw clean package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]

