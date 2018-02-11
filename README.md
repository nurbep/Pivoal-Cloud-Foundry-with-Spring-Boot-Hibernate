# Pivoal-Cloud-Foundry-with-Spring-Boot-Hibernate

## To make jar file 
- use maven build and type package in the goal 

## manifest.yml file
add some properties here to push Pivotal Cloud:  applications:
- name: ApexTest
path: target\ApexTest-0.0.1-SNAPSHOT.jar
buildpack: https://github.com/cloudfoundry/java-buildpack.git
memory: 1G
services:
  - ApexDatas
env:
  spring_jpa_hibernate_ddl-auto: update


## push your app  to PCF 
goto to app root directory using cd  and use " cf push appname " 
