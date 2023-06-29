FROM openjdk:17-jdk-alpine

 

COPY /Application/code/target/auth-service.jar ./

 

EXPOSE 8080

 

ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "-Dspring-boot.profiles.active=${JAVA_ENVIRONMENT}", "/ms-modele-auth.jar"]