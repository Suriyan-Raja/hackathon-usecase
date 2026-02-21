FROM maven:3.9-eclipse-temurin-17

WORKDIR /app

COPY pom.xml .
COPY src ./src

RUN mvn clean package -DskipTests

EXPOSE 8080

ENV PORT=3001

CMD ["java", "-jar", "target/order-service-0.0.1-SNAPSHOT.jar"]
