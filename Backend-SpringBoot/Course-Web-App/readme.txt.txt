# Swagger API enabled with basic config

## Dependencies Needed


```
<dependency>
    <groupId>io.springfox</groupId>
    <artifactId>springfox-boot-starter</artifactId>
    <version>3.0.0-SNAPSHOT</version>
</dependency>

<dependency>
    <groupId>io.springfox</groupId>
    <artifactId>springfox-swagger-ui</artifactId>
    <version>3.0.0-SNAPSHOT</version>
</dependency>
```
UI link --> http://localhost:8080/swagger-ui/

JSON docs --> http://localhost:8080/v3/api-docs

Example ref-> http://muralitechblog.com/swagger-rest-api-dcoumentation-for-spring-boot/
---------------------------------------------------------------------------------------------------
# What Is an Actuator?
In essence, Actuator brings production-ready features to our application.

Monitoring our app, gathering metrics, understanding traffic, or the state of our database become trivial with this dependency.

The main benefit of this library is that we can get production-grade tools without having to actually implement these features ourselves.

Actuator is mainly used to expose operational information about the running application — health, metrics, info, dump, env, etc. It uses HTTP endpoints or JMX beans to enable us to interact with it.


Getting Started
To enable Spring Boot Actuator, we just need to add the spring-boot-actuator dependency to our package manager.

In Maven:

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-actuator</artifactId>
</dependency>

In Application.properties
management.endpoints.web.exposure.include=*


Link to visit http://localhost:8080/actuator
---------------------------------------------------------------------------------------
# HAL explorer
Visualising with HAL explorer
2. HAL and the HAL Browser
JSON Hypertext Application Language, or HAL, is a simple format that gives a consistent and easy way to hyperlink between resources in our API. Including HAL within our REST API makes it much more explorable to users as well as being essentially self-documenting.

In Maven:
<dependency>
    <groupId>org.springframework.data</groupId>
    <artifactId>spring-data-rest-hal-explorer</artifactId>
    <version>3.4.1.RELEASE</version>
</dependency>


To access:
http://localhost:8080/

