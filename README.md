# Microservices communication via HTTP
This project have two applications : medicalFile and storeManagment

# DESCRIPTION
A medical file returned from the REST API of the service "medicalfile"  must contain the list of medications given to a patient.
Each medication in this list must be returned with its name. In order to get this information, the medicalfile service must ask 
the storeManagement service for this kind of data.

1- Implement the communication between the medical-file and the REST API of the store-management in order to get the names of the medications you need.

2- Use Swagger to document your API

3- Implement an exception handling mechanism to return a significant error message with a significant HTTP status code

4- Use docker to create a Docker image out of your application. After building the docker image, push it to the docker hub. Also,
you must run your docker image(start a container) and be able to interact with your application.

NOTE:
For those who want to use docker on windows 10, please follow this instructions 
https://docs.docker.com/docker-for-windows/wsl/

5- Use docker compose to improve the deployment of your system(the two microservices and databases).
Also you can try to use a maven plugin to build the docker images instead of using the docker build command.
https://docs.docker.com/compose/

# Architecture
![image](https://user-images.githubusercontent.com/78737274/107230551-81d9d800-6a1f-11eb-9cca-7c7a5b89c55e.png)

