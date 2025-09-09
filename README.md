# 🚪 API Gateway Service

**A Spring Boot–based API Gateway that routes requests to downstream microservices — simple, centralized, and production-ready.**

---

## ✨ Key Features

* **Gateway entrypoint** 🌐: Boots with `ApiGatewayApplication.java`.
* **Centralized configuration** ⚙️: Routes managed through `application.properties`.
* **Seamless routing** 🚦: Acts as a single entry point to microservices (e.g., Product, Payment, Email).
* **Lightweight** 🌱: No controllers or business logic — pure gateway responsibility.

---

## ⚡ Quickstart

Clone, build, and run:

```bash
git clone <this-repo>
cd api-gateway-service
mvn spring-boot:run
```

Default port: [http://localhost:8080](http://localhost:8080)

Configure routes in `application.properties`:

```properties
spring.cloud.gateway.routes[0].id=product-service
spring.cloud.gateway.routes[0].uri=http://localhost:8081
spring.cloud.gateway.routes[0].predicates[0]=Path=/products/**
```

---

## 🛠️ Tech Stack

* Java 21, Spring Boot 3.5
* Spring Cloud Gateway
* Maven

---

## 🧩 Architecture

* **ApiGatewayApplication** → Main entrypoint, sets up the Spring context.
* **Configuration** → `application.properties` defines routing rules.
* **Reverse Proxy** → Forwards incoming requests to appropriate downstream microservices.

---

## Link 

* [Apigateway](https://faithful-narwhal-cb8.notion.site/ApiGateway-26337b382b71805582a5d011fd8858dd) - Explained in detail

---

## 👤 Author

**Ramesh Nair**

* Backend Engineer | Java | Spring Boot | System Design Enthusiast
* Focused on building **scalable, maintainable, real-world systems**.
* Passionate about **clean architecture, design patterns, and domain modeling**.

📫 Reach me at: ramesh200212@gmail.com
🌐 GitHub: https://github.com/ramesh-nair-dev

