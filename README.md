# Uber-like Ride Booking Microservices Project

This repository serves as a **central reference** for my Uber-like ride-hailing microservices project built using **Java, Spring Boot, Redis, Kafka, WebSocket, and Eureka**. The project is divided into multiple microservices, each handling a specific responsibility.

---

## Project Overview

- **Type:** Backend Microservices  
- **Tech Stack:** Java, Spring Boot, Spring Security, JWT, Redis, Kafka, WebSocket, Eureka, JPA/Hibernate  
- **Description:** A scalable ride-booking system with real-time driver tracking, ride requests, and reviews. Each microservice is modular, deployable independently, and communicates asynchronously using Kafka and REST/WebSocket.

---

## Microservices

| Service | Description | GitHub Link |
|---------|-------------|-------------|
| **Booking Service** | Handles ride creation, driver assignment, and booking workflows | [Repo](https://github.com/JupiterBuilt369/UberProject-BookingService) |
| **Client WebSocket Service** | Manages real-time ride requests and driver responses | [Repo](https://github.com/JupiterBuilt369/UberProject-ClientWebSocketService) |
| **Frontend (STOMP)** | Frontend interface for passenger and driver interactions | [Repo](https://github.com/JupiterBuilt369/Stomp-Frontend) |
| **Service Discovery** | Eureka-based service registration and discovery | [Repo](https://github.com/JupiterBuilt369/UberProject-ServiceDiscovery) |
| **Location Service** | Handles driver geolocation storage and nearby driver queries | [Repo](https://github.com/JupiterBuilt369/UberProject-LocationService) |
| **Entity Service** | Centralized database models and repositories for passengers, drivers, and bookings | [Repo](https://github.com/JupiterBuilt369/UberProject-EntityService) |
| **Review Service** | Manages driver and passenger reviews | [Repo](https://github.com/JupiterBuilt369/UberProject-ReviewService) |
| **Auth Service** | Handles user authentication, JWT token management, and authorization | [Repo](https://github.com/JupiterBuilt369/UberProject-AuthService) |

---

## Key Features

- **Microservice Architecture**: Independent services communicating via REST and Kafka.  
- **Authentication & Authorization**: JWT-based security with Spring Security.  
- **Real-Time Updates**: WebSocket (STOMP over SockJS) for live ride and driver location updates.  
- **Location Tracking**: Redis GEO for nearby driver search and geospatial queries.  
- **Asynchronous Messaging**: Kafka for event-driven communication between services.  
- **Scalability**: Modular microservices deployed independently, registered via Eureka.  

---

## Usage

1. Clone individual repositories or fork the GitHub organization.  
2. Build using **Gradle** or **Maven**.  
3. Run services in the following order for full functionality:
   1. Entity Service  
   2. Service Discovery (Eureka)  
   3. Auth Service  
   4. Location Service  
   5. Booking Service  
   6. Review Service  
   7. Client WebSocket Service  
   8. Frontend (STOMP)  
4. Ensure **Redis** and **Kafka** are running locally or via Docker.  
5. Access frontend via STOMP client for ride requests and real-time updates.  

---

## Author

**Shivam Chaturvedi** – 
[GitHub Profile](https://github.com/JupiterBuilt369)  

---

# UberProject-Combined
