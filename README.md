# 🚗 RideSync/Uber Microservices Architecture

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

### Architecture Diagram
![Architecture Diagram](https://github.com/prachi310/uber-microservices-project/blob/main/uber%20project%20Architecture%20Diagram.drawio.png)

## Results
![EurekaService](https://github.com/prachi310/uber-microservices-project/blob/main/Eureka%20Result.png)

![BookingService](https://github.com/prachi310/uber-microservices-project/blob/main/Booking_service_driverRequest.png)

![BookingService](https://github.com/prachi310/uber-microservices-project/blob/main/Booking_service_driverReqID.png)

## 🔧 Setup and Running Instructions

1. **Clone Repositories**: Clone each microservice repository from GitHub.
2. **Set Up Eureka Server**: Start the Eureka server for service discovery.
3. **Configure Databases**: Ensure Redis,MYSQL and kafka are set up and running.
4. **Run Microservices**: Start each microservice as per their individual README instructions.
5. **Kafka Setup**: Ensure Kafka server is up and running for asynchronous communication.

## 📬 Postman Collections

To facilitate testing of the API endpoints for each microservice, we have created separate Postman collections. You can download and import these collections into Postman to quickly test the APIs.

### Download Postman Collections

- [Location Service](https://github.com/prachi310/uber-microservices-project/blob/main/UberLocationService.postman_collection.json)
- [Booking Service](https://github.com/prachi310/uber-microservices-project/blob/main/UberBookingService.postman_collection.json)
- [Socket Service](https://github.com/prachi310/uber-microservices-project/blob/main/UberSocketServer.postman_collection.json)
- [Review Service](https://github.com/prachi310/uber-microservices-project/blob/main/UberReviewService.postman_collection.json)
- [Auth Service](https://github.com/prachi310/uber-microservices-project/blob/main/UberAuthService.postman_collection.json)

### Importing Collections

1. **Open Postman**: Download and install Postman from [Postman](https://www.postman.com/downloads/).
2. **Import Collections**:
   - Click on `File` -> `Import`.
   - Select the downloaded Postman collection JSON files.
3. **Run Requests**: Use the imported collections to test the endpoints.




