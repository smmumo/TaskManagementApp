# Task Management Using Clean Architecture AND CQRS  

Event-driven task management system built using .NET 9, and Postgress, following clean architecture principles

What's included ?

- SharedKernel project with common Domain-Driven Design abstractions.
- Domain layer with sample entities.
- Application layer with abstractions for:
  - CQRS
  - Example use cases
  - Cross-cutting concerns (logging, validation)
- Infrastructure layer with:
  - Authentication
  - Permission authorization
  - EF Core, PostgreSQL
  - Serilog
- Seq for searching and analyzing structured logs
  - Seq is available at http://localhost:8081 by default
- Testing projects
  - Architecture testing

- API: Exposes REST endpoints to interact with tasks (Create, Update, Complete).
- Application: Contains CQRS command/query handlers and business logic.
- Domain: Defines aggregates, entities, and encapsulates domain logic.
- Infrastructure: Handles  SQL persistence, and external dependencies

- Domain-Driven Design
- Role-based authorization
- Permission-based authorization
- Distributed caching with Redis
- OpenTelemetry
- Outbox pattern
- API Versioning
- Unit testing
- Functional testing
- Integration testing

 ⚙️ Tech Stack
  - Layer	Tool / Library
  - Framework	.NET 9
  - Messaging	Apache Kafka via Docker
  - Persistence	Entity Framework Core + SQL Server
  - Mediation	MediatR
  - Resilience	Polly
  - Observability	K6, InfluxDB, Grafana
  - DevOps	Docker, Docker Compose
