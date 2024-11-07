# Ecommerce Website - Microservices Architecture

Welcome to my eCommerce project! This platform is built using a microservices architecture, designed to manage essential eCommerce functionalities such as product browsing, user authentication, payment handling, and notifications. Each service operates independently, which makes the platform scalable, resilient, and easy to maintain.

## Project Overview

This platform is divided into several microservices, each responsible for a key aspect of the eCommerce flow:

- **User Service**: Handles user registration, login, and authentication via OAuth 2.0.
- **Product Catalog Service**: Manages product listings and provides efficient product search using ElasticSearch.
- **Payment Gateway Service**: Processes secure payments using Razorpay.
- **Email Notification Service**: Automatically sends a welcome email to users upon registration using Kafka.

Each service can be tested independently, and they communicate with each other through REST APIs, Redis caching, and Kafka messaging.

## Individual Service Repositories

The project is split into separate repositories for each microservice. You can explore them individually:

- [**User Service**](https://github.com/sandhya7797/UserService): Manages user authentication and authorization via OAuth 2.0.
- [**Product Catalog Service**](https://github.com/sandhya7797/ThirdPartyAPI): Handles product management and search functionality with ElasticSearch integration.
- [**Payment Gateway Service**](https://github.com/sandhya7797/PaymentApplication): Secure payment processing with Razorpay integration.
- [**Email Notification Service**](https://github.com/sandhya7797/EmailNotificationService): Sends automated emails using Kafka upon user registration.

## Technical Architecture

This platform uses a microservices-based approach to separate concerns and ensure high availability and scalability:

- **Spring Boot & Spring Cloud**: For creating and managing the microservices.
- **OAuth 2.0**: Implemented for secure user authentication and authorization.
- **Redis Caching**: To reduce response times and improve performance.
- **ElasticSearch**: Used for efficient product searching and filtering.
- **Kafka**: Enables event-driven communication, particularly for sending notifications via email.
- **Razorpay**: Integrates with the payment service to handle secure transactions.

Here’s a high-level architecture diagram to visualize how everything fits together:

![Architecture Diagram](#path-to-your-architecture-diagram.png)

## Testing the Platform

While end-to-end flows aren’t set up for external testing, each service can be tested independently. Here’s how you can test each service:

- **User Service**: Test user registration and login using OAuth 2.0.
  - Example API: `POST /register` and `POST /login`
- **Product Catalog Service**: Test product search and filtering.
  - Example API: `GET /products?filter=...`
- **Payment Gateway Service**: Test payment processing.
  - Example API: `POST /payments`
- **Email Notification Service**: Verify that Kafka sends a welcome email after user registration.
  - Example: Trigger the `POST /register` endpoint to register a user and check email delivery.

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
- **Email Notification**: Kafka for sending automated emails on user registration

## Future Improvements

Here are a few ideas for future enhancements:

- Implement a recommendation engine to personalize product suggestions.
- Add SMS notifications in addition to email notifications.
- Enhance caching strategy with Redis clustering for even better performance.

## Contact

Feel free to reach out if you’d like to discuss this project or have any questions:

- [LinkedIn](https://www.linkedin.com/in/sandhya-ragulapadu-040007146/)
- [Email](mailto:ragulapadusandhya7797@gmail.com)
