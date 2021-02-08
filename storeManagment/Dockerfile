FROM openjdk:11
RUN apt-get update && apt-get install nmap -y
#RUN addgroup -S iit && adduser -S iit -G iit
#USER racem:racem
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} storeManagment-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["java","-jar","/storeManagment-0.0.1-SNAPSHOT.jar"]