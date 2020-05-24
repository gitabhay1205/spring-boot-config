# spring-boot-config
This is the Example of an Application whose Properties are fetched from config server.

Config Server
Application - spring-cloud-config-server(run this application - it will fetch all property files from ConfigServerProp)

Property file kept in
ConfigServerProp

If you make any changes to property file in ConfigServerProp, then hit the below endpoint

http://localhost:8080/actuator/refresh - It will refresh all the properties changed in the file.
