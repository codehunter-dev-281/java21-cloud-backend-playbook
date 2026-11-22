# Java 21 Cloud Backend Playbook

Practical examples and engineering notes for building
reliable, scalable Java backend applications.

## Tech Stack

- Java 21
- Spring Boot 3
- Spring Security
- PostgreSQL
- Apache Kafka
- Redis
- React & TypeScript
- Docker & Kubernetes
- AWS
- Azure OpenAI

## Engineering Focus

This project explores:

- REST API design and microservices
- Event-driven architecture with Kafka
- Authentication with OAuth 2.0 and JWT
- PostgreSQL performance optimization
- Cloud-native application deployment
- AI integration and Retrieval-Augmented Generation

## About

A collection of practical patterns and technical
notes inspired by real-world full-stack engineering.

All examples are independent educational material.

## Event-Driven Architecture

### Kafka-Based Order Processing

A typical event-driven order processing workflow:

1. Client submits an order through REST API.
2. Spring Boot validates the order request.
3. PostgreSQL stores the order transaction.
4. Kafka publishes an order-created event.
5. Inventory service processes the event.
6. Redis supports temporary inventory reservations.
7. Order status is updated asynchronously.

### Reliability Considerations

- Idempotent event processing
- Retry handling and dead-letter topics
- Transactional outbox pattern
- Distributed tracing
- Monitoring and alerting

### Design Goals

Build resilient microservices that can handle
high traffic without duplicate order processing.
