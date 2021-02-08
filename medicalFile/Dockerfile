FROM openjdk:11
#RUN addgroup -S iit && adduser -S iit -G iit
#USER racem:racem
#ARG JAR_FILE=target/*.jar
#COPY ${JAR_FILE} medicalFile-0.0.1-SNAPSHOT.jar
#RUN apt-get update && apt-get install dnsutils -y
#ENTRYPOINT ["java","-jar","/medicalFile-0.0.1-SNAPSHOT.jar"]
ARG DEPENDENCY=target/dependency
COPY ${DEPENDENCY}/BOOT-INF/lib /app/lib
COPY ${DEPENDENCY}/META-INF /app/META-INF
COPY ${DEPENDENCY}/BOOT-INF/classes /app
ENTRYPOINT ["java","-cp","app:app/lib/*","tn.iit.MedicalFileApplication"]

