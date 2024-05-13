# Nest Backend

This framework aims at separation of concerns so we have:

1. [Modules](#modules)
2. [Controllers](#contollers)
3. [Services](#services)

## Modules

Modules are the fundamental building blocks in NestJS. They are used to organize the application structure. Each module encapsulates providers, controllers, and other related code. Everything related to a specific feature set, such as a user management, can be encapsulated in a single module.

### Purpose:

- Organize related features together (like a container).
- Encapsulate the application functionality.
- Facilitate modularity and reusability.

## Controllers

Controllers are responsible for handling incoming requests and returning responses to the client. They bind the application's logic to different HTTP routes. Controllers in NestJS are defined with decorators that help route the requests and provide other metadata needed to configure the routes properly.

### Purpose:

- Handle HTTP requests (GET, POST, PUT, DELETE, etc.).
- Validate input.
- Return responses.
- Act as an intermediary between the client(web/mobile app) and the services (application's backend logic).

## Services

Services (often referred to as providers in NestJS) are classes that encapsulate the core business logic of the application. They are used by controllers or other services. They are designed to be reusable throughout the application.

### Purpose:

- Encapsulate business logic.
- Share code across controllers.
- Isolate functionality (making testing easier).
