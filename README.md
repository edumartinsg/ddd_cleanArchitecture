# Project Description

## Project based on clean architecture and Domain drive design

## What is DDD and Clean Archictecture?

## Domain-Driven Design (DDD)

Domain-Driven Design (DDD) is an approach to software development that focuses on the business domain and its logic. It emphasizes collaboration between technical experts and domain experts to create software that accurately reflects the real-world problems it is intended to solve. Here are the key concepts:

- Domain: The core business logic and rules that define your application.

- Entities: Objects that have a unique identity and persist throughout the application. For example, a User or Order.

- Value Objects: Objects that do not have a unique identity and are defined by their attributes. For example, Address or Money.

- Aggregates: A cluster of domain objects that can be treated as a single unit. Each aggregate has a root entity known as the Aggregate Root.

- Repositories: Interfaces that provide access to aggregate roots. They abstract the database operations.

- Services: Domain services encapsulate business logic that doesn’t naturally fit within an entity or value object.

- Ubiquitous Language: A common language used by both developers and domain experts to ensure clear communication and understanding.

- Bounded Context: A boundary within which a particular domain model is defined and applicable. It helps in managing complexity by dividing the system into smaller parts.

## How to Use DDD in a Backend Project

Understand the Domain: Collaborate with domain experts to understand the business logic and define the ubiquitous language.

Identify Entities and Value Objects: Determine the main entities and value objects that represent the domain.

Define Aggregates: Group related entities and value objects into aggregates and establish aggregate roots.

Create Repositories: Implement repositories to manage aggregate roots and abstract data access.

Implement Domain Services: Use domain services for complex business logic that spans multiple entities or aggregates.

Establish Bounded Contexts: Divide your application into bounded contexts to manage complexity and ensure that each context has its own model.

## Clean Architecture

Clean Architecture is a software design philosophy that aims to make your software easier to understand, maintain, and test by separating concerns and dependencies. It’s structured around several key principles:

- Separation of Concerns: Divide your application into layers, each with a specific responsibility.

- Independence: Your business logic should be independent of external frameworks, databases, and UI. This allows for flexibility and easier testing.

- Dependency Inversion: Higher-level modules should not depend on lower-level modules; both should depend on abstractions.

- Entities: Core business logic and rules. They should be independent of any external influence.

- Use Cases: Application-specific business rules. They orchestrate the flow of data to and from the entities.

- Interfaces: Define contracts for external systems, databases, and UI interactions.

- Adapters: Translate data between the application and external systems. This includes APIs, databases, and user interfaces.

- Frameworks and Drivers: External tools and frameworks that interact with the application. They should be at the outermost layer.

## How to Use Clean Architecture in a Backend Project

Define Core Entities: Identify and define the entities that encapsulate your core business logic.

Develop Use Cases: Implement application-specific logic that uses entities to achieve business goals.

Create Interfaces: Define interfaces for all external interactions, such as databases, APIs, and UI components.

Implement Adapters: Write code to convert data between your application’s internal structures and external interfaces.

Use Dependency Injection: Inject dependencies into your classes rather than hardcoding them, promoting flexibility and testability.

Organize Layers: Arrange your code into layers based on responsibility, typically:

Entities (Core Layer): Contains business rules.

Use Cases (Application Layer): Contains application-specific business logic.

Interfaces (Interface Layer): Defines contracts for external systems.

Adapters (Adapter Layer): Implements interface contracts and handles external system interactions.

![alt text](./imgs/image.png)

# Other used patterns

## Functional Error Handling

## Aggregates & Watched Lists
