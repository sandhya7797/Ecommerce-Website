# Ecommerce-Website

Welcome to my eCommerce platform project! This platform is built using a microservices architecture, designed to manage essential eCommerce functionalities such as product browsing, order processing, payment handling, and notifications. Each service operates independently, which makes the platform scalable, resilient, and easy to maintain.

## Project Overview

This platform is divided into several microservices, each responsible for a key aspect of the eCommerce flow:

- **Product Catalog Service**: Manages product listings and provides efficient product search using ElasticSearch.
- **Order Service**: Handles the order lifecycle from creation to tracking.
- **Payment Gateway Service**: Processes secure payments using Razorpay.
- **Notification Service**: Sends event-driven email notifications using Kafka.

Each service can be tested individually, and they communicate with each other through REST APIs, Redis caching, and Kafka messaging.

## Individual Service Repositories

The project is split into separate repositories for each microservice. You can explore them individually:

- [**Product Catalog Service**](link-to-product-service-repo): Handles product management and search functionality with ElasticSearch integration.
- [**Order Service**](link-to-order-service-repo): Manages order creation, tracking, and updates.
- [**Payment Gateway Service**](link-to-payment-service-repo): Secure payment processing with Razorpay integration.
- [**Notification Service**](link-to-notification-service-repo): Event-driven notification service using Kafka for communication.

## Technical Architecture

This platform uses a microservices-based approach to separate concerns and ensure high availability and scalability:

- **Spring Boot & Spring Cloud**: For creating and managing the microservices.
- **Redis Caching**: To reduce response times and improve performance.
- **ElasticSearch**: Used for efficient product searching and filtering.
- **Kafka**: Enables event-driven communication, particularly for sending notifications.
- **Razorpay**: Integrates with the payment service to handle secure transactions.

Here’s a high-level architecture diagram to visualize how everything fits together:

![Architecture Diagram](path-to-your-architecture-diagram.png)

## Getting Started

To get started with the platform, follow the steps below to set up each service on your local machine.

1. **Clone the repositories**: Download the individual repositories (linked above) to your local machine.
   
2. **Set up prerequisites**: Make sure MySQL, Redis, and Kafka are installed and running locally.

3. **Run the services**:
   - Navigate to each service directory and run the following command to start the microservice:
     ```bash
     mvn spring-boot:run
     ```
   
   - Repeat this for each microservice (Product, Order, Payment, Notification).

4. **Explore APIs**: Each service exposes a set of REST APIs. You can interact with them directly via Postman or Curl.

   - **Product Catalog**: `GET /products` (with filtering options)
   - **Order Service**: `POST /orders` (to create an order)
   - **Payment Service**: `POST /payments` (to process a payment)
   - **Notification Service**: Use Kafka to trigger events for email notifications.

## Testing the Platform

While end-to-end flows aren’t set up for external testing, each service can be tested independently. Here’s how you can test each service:

- **Product Catalog Service**: Test product search and filtering.
  - Example API: `GET /products?filter=...`
- **Order Service**: Test order creation and tracking.
  - Example API: `POST /orders`
- **Payment Gateway Service**: Test payment processing.
  - Example API: `POST /payments`
- **Notification Service**: Trigger email notifications via Kafka events.

For detailed API documentation and usage, check out the individual repositories.

## Technologies Used

This project is built using the following technologies:

- **Backend**: Spring Boot, Spring Cloud
- **Database**: MySQL
- **Caching**: Redis
- **Messaging**: Kafka
- **Search**: ElasticSearch
- **Payments**: Razorpay

## Future Improvements

Here are a few ideas for future enhancements:

- Implement a recommendation engine to personalize product suggestions.
- Add SMS notifications in addition to email notifications.
- Enhance caching strategy with Redis clustering for even better performance.

## Contact

Feel free to reach out if you’d like to discuss this project or have any questions:

- [LinkedIn](https://linkedin.com/in/yourusername)
- [Email](mailto:email@example.com)


