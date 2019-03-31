# a spring boot based templet for developing web service
It is a maven project, and the original project is [here](https://github.com/ityouknow/spring-boot-examples/tree/master/spring-boot-docker)  
## program your own service
1. modify src/main/java/com/neo/controller/DockerController.java by adding your algorithm in function "method"  
2. run start class: src/main/java/com/neo/DockerApplication.java. To test your service, invoke "http://localhost:8080"
## make a docker image
1. customize the docker image name in line 7 of file pom.xml  
2. modify dockerfile: src/main/docker/Dockerfile  
3. install and configure Docker, JDK and Maven  
4. enter you project path and run command "mvn package docker:build"  
5. if success, run command "docker images" and you will see the new docker image  
