# Ecommerce Website - Microservices Architecture

Welcome to my Ecommerce platform project! This platform is built using a microservices architecture, designed to manage essential ecommerce functionalities such as product browsing, payment handling, user authentication, and notifications. Each service operates independently, which makes the platform scalable, resilient, and easy to maintain.

## Project Overview

This platform is divided into several microservices, each responsible for a key aspect of the eCommerce flow:

- **User Service**: Handles user registration, login, and authentication via OAuth 2.0.
- **Product Catalog Service**: Manages product listings and provides efficient product search using ElasticSearch.
- **Payment Gateway Service**: Processes secure payments using Razorpay.
- **Notification Service**: Sends event-driven email notifications using Kafka.

Each service can be tested independently, and they communicate with each other through REST APIs, Redis caching, and Kafka messaging.

## Individual Service Repositories

The project is split into separate repositories for each microservice. You can explore them individually:

- [**User Service**](link-to-user-service-repo): Manages user authentication and authorization via OAuth 2.0.
- [**Product Catalog Service**](link-to-product-service-repo): Handles product management and search functionality with ElasticSearch integration.
- [**Payment Gateway Service**](link-to-payment-service-repo): Secure payment processing with Razorpay integration.
- [**Notification Service**](link-to-notification-service-repo): Event-driven notification service using Kafka for communication.

## Technical Architecture

This platform uses a microservices-based approach to separate concerns and ensure high availability and scalability:

- **Spring Boot & Spring Cloud**: For creating and managing the microservices.
- **OAuth 2.0**: Implemented for secure user authentication and authorization.
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
   
   - Repeat this for each microservice (User, Product, Payment, Notification).

4. **Explore APIs**: Each service exposes a set of REST APIs. You can interact with them directly via Postman or Curl.

   - **User Service**: Authentication via OAuth 2.0 (e.g., `POST /login`, `POST /register`)
   - **Product Catalog**: `GET /products` (with filtering options)
   - **Payment Service**: `POST /payments` (to process a payment)
   - **Notification Service**: Use Kafka to trigger events for email notifications.

## Testing the Platform

While end-to-end flows aren’t set up for external testing, each service can be tested independently. Here’s how you can test each service:

- **User Service**: Test user registration and login using OAuth 2.0.
  - Example API: `POST /register` and `POST /login`
- **Product Catalog Service**: Test product search and filtering.
  - Example API: `GET /products?filter=...`
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
- **Authentication**: OAuth 2.0 for secure user login and authorization

## Future Improvements

Here are a few ideas for future enhancements:

- Implement a recommendation engine to personalize product suggestions.
- Add SMS notifications in addition to email notifications.
- Enhance caching strategy with Redis clustering for even better performance.

## Contact

Feel free to reach out if you’d like to discuss this project or have any questions:

- [LinkedIn](https://linkedin.com/in/yourusername)
- [Email](mailto:email@example.com)



