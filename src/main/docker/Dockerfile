FROM openjdk:8u111-jre-alpine
VOLUME /tmp
ADD gs-serving-web-content-0.1.0.jar /app.jar
RUN sh -c 'touch /app.jar'
EXPOSE 8080
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]