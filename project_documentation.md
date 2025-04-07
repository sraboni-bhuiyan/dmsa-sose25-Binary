# Instant Mobility Platform

## Summary

A platform that bundles mobility offers from various providers, enabling users to search, book, and pay for vehicles directly.

Key Features:

- User and provider account management.
- Vehicle registration, management, and booking.
- Payment processing and user reviews.
- Microservice architecture using Java/Kotlin and Spring.

## Functionality

### Functional requirements

{
Description of the application functions you have implemented with reference to the task of the scenario (_Lab Assignment 2, Task 2.1_)
}

For Providers:
- Register, view, edit, and delete vehicles.
- Define vehicle types, pricing, and restrictions.
- Monitor fleet status (location, availability).

For Users:
- Search for vehicles by location and filters.
- Book and terminate vehicle usage.
- Make payments and leave ratings.
- View booking history.


**Schema for Requirements:**
  - **Unique Identifier:** (e.g., FR-01)
  - **Name:** (e.g., Vehicle Registration)
  - **Description:** (e.g., Providers can register vehicles for rental on the platform.)
  - **Priority:** (e.g., High)
  - **Actors/Roles:** (e.g., Providers)

**Requirements List:**
  - **FR-01:** Vehicle Registration
    - Description: Providers can register vehicles for rental on the platform.
    - Priority: High
    - Actors/Roles: Providers
  - **FR-02:** Vehicle Search
    - Description: Users can search for available vehicles based on location and filters.
    - Priority: High
    - Actors/Roles: Users


### Description of the domain concepts (domain model)

{
Description of the domain concepts in the form of one or more DDD models and textual explanation (_Lab Assignment 2, Task 2.2; Lab Assignment 3; Lab Assignment 4_)
}

Domain Model:
- Explanation of key entities like User, Provider, Vehicle, Booking, and Payment.
- UML diagrams for relationships between entities.

DDD Models:
- Bounded contexts for user management, vehicle management, and booking/payment.

## Architecture design

{
Describe the design of your architecture here, e.g. using UML models (class diagrams of the domain concepts, component diagrams of the microservice artifacts, deployment diagrams, etc.) and textual explanations.
}

Microservice Architecture:
- Overview of services: User Service, Provider Service, Vehicle Service, Booking Service, Payment Service.
- Component diagrams for service interactions.

Deployment Diagram:
- Cloud-based deployment with load balancers, databases, and service instances.

Technology Stack:
- Java/Kotlin with Spring Framework.
- PostgreSQL for the sample database.
- REST APIs for communication.

## Implementation

### Technologies

{
List the technologies you used to implement your architecture design, briefly describe the general purpose of each technology and why you chose that technology in light of your architecture design.
}

Technologies:
- Spring Framework: For building microservices.
- PostgreSQL: For managing the sample database.
- Docker: For containerization.
- Swagger/OpenAPI: For API documentation.


### Solution architecture

{
Describe the solution architecture of your application here, i.e. how you implemented your architecture design with which of the technologies used.
}

Solution Architecture:
- Explanation of how services interact to fulfill requirements.
- Example workflows for booking and payment.

--------------------------------------------------------------------------------
User Guide

For Providers:
Steps to register and manage vehicles.
Monitoring fleet status.
For Users:
Searching and booking vehicles.
Making payments and leaving reviews.

API Documentation

Endpoints:
users: User account management.
/providers: Provider account and vehicle management.
/vehicles: Vehicle search and filtering.
/bookings: Booking and termination.
/payments: Payment processing.
Sample Requests and Responses:
Example JSON payloads for each endpoint.

Database Design

ER Diagram:
Tables for Users, Providers, Vehicles, Bookings, and Payments.
Sample Data:
Predefined users, providers, and vehicles for testing.

Deployment:

Setup Instructions:
Steps to deploy the platform using Docker.
Environment variables and configuration files.
Running Locally:
Instructions for running the platform on a local machine.

Future Enhancements

Planned Features:
Integration with external payment gateways.
Support for additional vehicle types.
Advanced analytics for providers.