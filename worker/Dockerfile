FROM maven:3.8.4-jdk-11-slim AS builder

WORKDIR /app/worker

COPY . .

RUN mvn dependency:resolve

RUN mvn package

FROM openjdk:11-jre-slim

WORKDIR /app/worker

COPY --from=builder /app/worker/target/worker-jar-with-dependencies.jar .

EXPOSE 80

CMD ["java","-jar", "worker-jar-with-dependencies.jar"]