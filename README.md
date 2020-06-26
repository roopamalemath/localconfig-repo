# localconfig-repo

file name should be applicationname-envt.properties
Ex : limits-service-dev.properties

each microservice have assigned to different environment.
each enviroment have different instances of same microservice
all the different environment of different microservices are stored in spring cloud config server

enviroments such as dev, qa, prod, stage and default etc....

To check where the spring-cloud-config-server able to acceess the git repo(where all the property stored in git repo)
localhost:8888/limits-service/qa
localhost:8888/limits-service/prod
localhost:8888/limits-service/dev
localhost:8888/limits-service/default 



propertysources are in the order of priorities
the value which was inside the default but which was not present in dev.properties. then the value from the efault will be picked up.
