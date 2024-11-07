# Ecommerce-Website

A comprehensive eCommerce platform built with a microservices architecture to handle essential eCommerce functionalities, optimized for performance and scalability.

## Overview

This project consists of multiple microservices, each hosted in its own repository, including:

- **Product Catalog Service**: Manages product listings and enables search with ElasticSearch.
- **Order Service**: Handles order creation, tracking, and management.
- **Payment Gateway Service**: Processes payments via Razorpay.
- **Notification Service**: Manages notifications, leveraging Kafka for event-driven email distribution.

## Repositories

Each microservice is housed in its own repository. Here’s a quick guide to each:

- [**Product Catalog Service**](link-to-product-service-repo): Contains the product catalog, integrated with ElasticSearch for efficient product discovery.
- [**Order Service**](link-to-order-service-repo): Manages the entire order lifecycle.
- [**Payment Gateway Service**](link-to-payment-service-repo): Integrates with Razorpay for secure payments.
- [**Notification Service**](link-to-notification-service-repo): Sends notifications and uses Kafka for event-driven processing.

## Architecture

This platform uses a microservices approach, designed with Spring Boot and Spring Cloud. Redis is used for caching to improve performance, and Kafka enables asynchronous communication between services.

![Architecture Diagram](path-to-your-architecture-diagram.png)

## Quick Start

To run each service, follow the instructions in the linked repositories above. Key setup steps include:

1. Clone each repository.
2. Set up MySQL, Redis, and Kafka locally.
3. Start each service individually by navigating to the service directory and running `mvn spring-boot:run`.

## Technologies Used

- **Backend**: Spring Boot, Spring Cloud
- **Database**: MySQL
- **Caching**: Redis
- **Messaging**: Kafka
- **Search**: ElasticSearch
- **Payments**: Razorpay

## Contact

Reach me on [LinkedIn](https://linkedin.com/in/yourusername) or via [email@example.com](mailto:email@example.com).
