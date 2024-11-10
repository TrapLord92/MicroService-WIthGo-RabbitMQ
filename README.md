

---

# Distributed Microservice Architecture with Chi Framework

This project implements a distributed microservice architecture using the **Chi** framework, **Docker Compose**, and **Docker Swarm**. The architecture facilitates communication between microservices through various protocols and services.

## Services Overview

- **Broker (Entry Point)**: Acts as the main entry point to access all microservices.
- **Authentication**: User authentication data is securely stored in **PostgreSQL**.
- **Logger**: Logs data are saved to **MongoDB** for efficient querying and persistence.
- **Mail Service**: Sends templated emails using a customizable email template.
- **Listener**: A listener service that consumes messages from **RabbitMQ** for processing.
  
## Communication Protocols

- **REST API**: The microservices communicate via REST APIs using **JSON transport** for data exchange.
- **RPC & gRPC**: Remote Procedure Calls (RPC) and gRPC are used for efficient inter-service communication.
- **AMQP (Advanced Message Queuing Protocol)**: Events are initiated and responded to using AMQP for asynchronous communication between services.

## Key Features

- **Distributed Microservice Architecture**: Each microservice is encapsulated and managed using Docker Swarm for orchestration and scaling.
- **State Management**: 
  - Authentication data and user sessions are stored in PostgreSQL.
  - Logs and monitoring data are stored in MongoDB.
- **Message Queue**: RabbitMQ is used for consuming and processing events/messages in an asynchronous, scalable way.

## Technologies Used

- **Chi Framework**: A lightweight, idiomatic Go web framework for building RESTful APIs.
- **Docker & Docker Compose**: Used for containerizing services, managing local development environments, and scaling microservices with Docker Swarm.
- **PostgreSQL**: Relational database management system used to store authentication data.
- **MongoDB**: NoSQL database used to store log data.
- **RabbitMQ**: Message broker for enabling event-driven communication between services.
- **gRPC & RPC**: Efficient protocols for inter-service communication.
- **AMQP**: Protocol for sending and receiving events asynchronously.

---
