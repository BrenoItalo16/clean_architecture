# Clean Architecture - Flutter

This project was created to study and practice Clean Architecture in Flutter applications. Clean Architecture promotes a clear separation of concerns, leading to a more organized and scalable structure.

## Project Overview

The goal of this project is to implement a clean architecture that facilitates maintenance, testability, and scalability. This is achieved by separating business logic (domain), presentation logic (UI), infrastructure (data), and user interaction into distinct layers.

### Project Structure

The project follows a structure that reflects the principles of Clean Architecture:

- **core**: Contains entities, business rules, and use cases that do not depend on other layers.
- **data**: Repository implementations, APIs, local data sources, and data model mappings.
- **domain**: Defines entities and repository interfaces. Contains the use cases (interactors), which are the application logic.
- **presentation**: Contains Flutter widgets, controllers, state managers, and other UI-related classes.
- **dependency_injection**: Configuration of dependency injectors for each layer of the project.

## Technologies Used

- [Flutter](https://flutter.dev/) - Cross-platform application development framework.
- [Dart](https://dart.dev/) - Programming language used by Flutter.
- [GetIt](https://pub.dev/packages/get_it) - Dependency injection.
- [Freezed](https://pub.dev/packages/freezed) - Code generation for immutable classes.
- [Dartz](https://pub.dev/packages/dartz) - Functional programming tools for handling failures (Result, Either).

## Patterns and Principles

- **Dependency Injection**: All dependencies are resolved using the `GetIt` package, which improves testability and maintainability.
- **SOLID**: The project design follows SOLID principles to ensure high cohesion and low coupling.
- **TDD (Test Driven Development)**: Use cases were developed using unit tests to ensure robustness of business logic.

## How to Run the Project

1. **Clone the Repository:**

```bash
git clone https://github.com/BrenoItalo16/clean_architecture.git
