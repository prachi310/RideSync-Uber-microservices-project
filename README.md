# 🚗 Uber Microservices Architecture

This repository serves as the central hub for the Uber Microservices Architecture project, designed to showcase a robust and scalable ride-sharing application. Each microservice is built using Spring Boot and handles a specific functionality of the application.

## 🌟 Project Highlights

- **Real-time Driver Location Tracking**: Utilizes Redis for efficient real-time location updates and proximity searches.
- **Booking Management**: Comprehensive handling of ride bookings, ensuring reliability and performance.
- **Interactive Communication**: Real-time interactions via STOMP-based WebSockets for seamless client and service communication.
- **Robust Authentication**: Secure JWT token-based authentication implemented with Spring Security.
- **User Reviews**: Complete CRUD operations for managing driver and passenger reviews.
- **Service Discovery**: Dynamic service registration and discovery managed by Eureka.
- **Asynchronous Processing**: Kafka for robust and scalable asynchronous communication.
  

## 🛠️ Microservice Breakdown

### 1. [Location Service](https://github.com/prachi310/UberProject-LocationService.git)
  - **Purpose**: Manages and updates live driver locations; fetches nearby drivers.
  - **Stack**: Spring Boot, Redis

### 2. [Entity Service](https://github.com/prachi310/UberProject-EntityService.git)
- **Purpose**: Central repository for common models used across microservices.
- **Stack**: Spring Boot , 

### 3. [Booking Service](https://github.com/prachi310/UberProject-BookingService.git)
- **Purpose**: Manages all booking-related functionalities.
- **Stack**: Spring Boot, Spring Data JPA, Kafka

### 4. [Socket Service](https://github.com/prachi310/SocketServer-SpringBoot.git)
- **Purpose**: Manages real-time client-server communication using WebSockets.
- **Stack**: Spring Boot, Spring WebSocket
  
### 5. [Review Service](https://github.com/prachi310/UberProject-ReviewService.git)
- **Purpose**: Handles CRUD operations for user reviews.
- **Stack**: Spring Boot, Spring Data JPA

### 6. [Eureka Service Discovery](https://github.com/prachi310/UberProject-Eureka-Service-Discovery.git)
- **Purpose**: Service registry and discovery.
- **Stack**: Spring Boot, Eureka

### 7. [Auth Service](https://github.com/prachi310/UberProject-AuthService.git)
- **Purpose**: JWT token-based user authentication.
- **Stack**: Spring Boot, Spring Security


## ⚙️ Additional Infrastructure

- **Kafka:** Used for asynchronous service communication.
- **Retrofit:** For asynchronous API calls.
- **Spring Boot:** Core framework for all microservices.
- **Spring Data JPA:** For database operations.
- **Spring Socket, Spring Redis, Spring Kafka, Scheduler:** Various Spring modules used.
- **Flyway:** Database migration tool.

## 🚀 Technologies Used

- **Programming Language:** Java
- **Frameworks:** Spring Boot, Spring Security, Spring Data JPA, Spring Kafka, Spring Redis
- **Database:** Redis, MySQL
- **Messaging:** Kafka
- **API Communication:** Retrofit
- **Others:** Flyway for DB migration, STOMP for sockets

## 🔧 Setup and Running Instructions

1. **Clone Repositories**: Clone each microservice repository from GitHub.
2. **Set Up Eureka Server**: Start the Eureka server for service discovery.
3. **Configure Databases**: Ensure Redis and PostgreSQL are set up and running.
4. **Run Microservices**: Start each microservice as per their individual README instructions.
5. **Kafka Setup**: Ensure Kafka server is up and running for asynchronous communication.





