FROM openjdk:11
WORKDIR /usr/src/app
COPY spring-example-project .
EXPOSE 8080
VOLUME /tmp
RUN chmod a+rx ./target/docker-example-1.1.3.jar
ENTRYPOINT ["java","-jar","./target/docker-example-1.1.3.jar"]
