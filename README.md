# spring-boot-config
This is the Example of an Application whose Properties are fetched from config server.

Config Server
Application - spring-cloud-config-server(run this application - it will fetch all property files from ConfigServerProp)

Property file kept in
ConfigServerProp

If you make any changes to property file(right now active profile is uat, see in bootstrap file) in ConfigServerProp, then hit the below endpoint

http://localhost:8080/actuator/refresh - It will refresh all the properties changed in the spring-boot-congig-uat file.

Similary you can change properties in prod and dev files and mentioned that profile in bootStrap file of this program, so you will be able to test it.
