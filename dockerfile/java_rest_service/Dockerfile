FROM openjdk:8-jre-slim

MAINTAINER Pawel Skwarcz "p.skwarcz@gmail.com"

WORKDIR /home

COPY gs-rest-service-0.1.0.jar gs-service.jar

ENTRYPOINT ["java","-jar", "gs-service.jar"]

EXPOSE 8080
