# ECommerce Microservices Platform

A scalable microservices-based backend system built with Java Spring Boot, demonstrating secure user management, provider operations, and email notifications across services.

## 🔧 Architecture Overview

This project is composed of three independent services communicating over HTTP and secured using OAuth2. It showcases core components of a distributed e-commerce system.

---

## 📦 Microservices

### 1. 🔐 [UserService](./UserService)
- Handles user registration, login, and role-based access.
- Secured using **Spring Security + OAuth2 Resource Server**.
- Exposes REST APIs for user CRUD operations.
- Supports **JWT-based authentication** and **scope validation**.

### 2. 🏬 [ProviderService](./ProviderService)
- Simulates vendor/product-provider functionalities.
- Communicates securely with UserService using **OAuth2 tokens**.
- Protected with **Role-Based Access Control (RBAC)**.
- Contains business logic for managing provider-specific resources.

### 3. 📧 [EmailService](./EmailService)
- Event-driven email notification system.
- Listens to events from other services and sends templated emails.
- Built for horizontal scalability.
- Integrates with third-party mail clients (e.g., SMTP, SendGrid-ready).

---

## 🔐 Security
- **OAuth2 Resource Server** and **Authorization Server integration**.
- Uses **JWT tokens** with role and scope validation.
- Enforces secure inter-service communication via token headers.

---

## ⚙️ Tech Stack
- Java 17, Spring Boot 3+
- Spring Security, Spring Data JPA, Redis
- MySQL, Maven, REST APIs
- OAuth2, JWT
- Docker-ready setup (optional)
- Postman Collection (available for API testing)

---

## 🚀 Getting Started
1. Clone the repository
2. Configure MySQL for each service
3. Run each microservice from its module directory
4. Use Postman collection to test secured endpoints

---

## 📈 Future Enhancements
- API Gateway & Service Discovery using Spring Cloud
- Order Service as a Mircroservice
- Enhance monitoring with tools like Prometheus and Grafana.

---

##  🚀 Getting Started
### Clone the project and initialize submodules
```bash
git clone https://github.com/rahulkotha07/ECommerce-Microservices.git
cd ECommerce-Microservices
git submodule update --init --recursive

```

### 📌 Author
**Rahul Kotha**  
[LinkedIn](https://www.linkedin.com/in/rahul--kotha) | [Email](mailto:rahulkotha07@gmail.com)

