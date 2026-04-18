# customer-service

Customer microservice for the e-commerce sample platform. It stores customer data, loads shared configuration from the config server, and registers itself in Eureka.

## Responsibilities

- customer persistence with Spring Data JPA
- REST exposure of customer resources
- configuration refresh and config inspection endpoints
- integration with central config and service discovery

## Stack

- Java 17
- Spring Boot
- Spring Data JPA / Data REST
- H2 Database
- Spring Cloud Config Client
- Eureka Client
- Spring Boot Actuator

## Useful Endpoints

- `/customers`
- `/testConfig`
- `/globalConfig`

## Default Configuration

- Port: `8081`
- Config server: `CONFIG_SERVICE_URL`, defaulting to `http://localhost:9999`

## Run Locally

```bash
./mvnw spring-boot:run
```
