Kubernetes Deployment Files

This repository contains all kubernetes files needed to deploy the Lenneflow application in a kubernetes environement.
In order to make a correct deployment, please edit the files to meet the write configurations.

In the secret files, please provide the base64 encoded secret for working mongodb and rabbitmq installations.
- spring.data.mongodb.username:
- spring.data.mongodb.password:
- rabbit.username:
- rabbit.password:
  
Lenneflow uses rabbitmq for message transmission between pods and data are saved in a mongodb database.
Both mongodb and rabbitmq users must have enough rights to read and write files. In best case, give admin rights.

In the configmap files please adapt the configuration. Rabbitmq and Mongodb configuration must be updated
- spring.data.mongodb.host=[mongodb host name]
- rabbit.address=[rabbitmq host name]
- rabbit.port=[mongodb port]
