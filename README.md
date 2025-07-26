# 📚 Project: Spring Boot Microservices Bookstore

This project is a microservices-based **Bookstore Application** built with **Spring Boot**, **Spring Cloud**, **Keycloak**, and **Docker**. It showcases my understanding of building scalable, secure, and resilient backend systems using modern Java frameworks.


![BookStore Microservices Architecture](docs/bookstore-spring-microservices.png)

---

## 🧩 Project Modules & Tech Stack

### 🗂️ catalog-service
Manages the catalog of books (CRUD APIs).  
**Stack**: Spring Boot, Spring Data JPA, PostgreSQL

### 📦 order-service
Handles order processing and publishes events to RabbitMQ.  
**Stack**: Spring Boot, Spring Security OAuth2, Keycloak, Spring Data JPA, PostgreSQL, RabbitMQ

### 📢 notification-service
Listens for order events and sends user notifications.  
**Stack**: Spring Boot, RabbitMQ

### 🚪 api-gateway
Routes and secures traffic to backend services.  
**Stack**: Spring Cloud Gateway, Spring Boot

### 🌐 bookstore-webapp
Customer-facing web UI to browse, order, and view books.  
**Stack**: Spring Boot, Thymeleaf, Keycloak, Alpine.js, Bootstrap

---

## 🎯 Project Objectives

- Building RESTful services with Spring Boot
- Asynchronous communication with RabbitMQ
- OAuth2 and Role-based Access Control using Keycloak
- Using API Gateway for routing and security
- Database versioning with Flyway
- Distributed job scheduling with ShedLock
- Containerized local development with Docker and Testcontainers
- Writing integration and contract tests with JUnit, RestAssured, and WireMock
- Centralized logging and observability with Grafana stack

---

## 🚀 Local Setup

To run this application locally:

1. Install Java 21 (I used [SDKMAN](https://sdkman.io/))
2. Install [Docker Desktop](https://www.docker.com/products/docker-desktop/)
3. Use an IDE like [IntelliJ IDEA](https://www.jetbrains.com/idea)
4. Clone the repository and run:

```bash
docker-compose up --build





