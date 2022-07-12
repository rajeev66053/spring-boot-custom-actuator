# User Management App with custom Actuator and security

* For live reload the application on change on code use devtools dependency in pom.xml
* Actuator dependency is used to check the health of application. We can check by:
    > http://localhost:8082/actuator

* UserAppInfoEndPoint is used for custom actuator endpoint creation. Which will be available in
    > http://localhost:8082/actuator/userAppInfo

* We can create actuator endpoint using controller end point. The end point will be added in actator. We can access it by below url where `message-from-solar` is get method
    > http://localhost:8082/actuator/controllerEndPoint/message-from-solar
  
* Use spring security to securing the actuator acess. By defualt it allow /health and /info.