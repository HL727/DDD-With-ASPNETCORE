# Diagram

## Overview
![](/Docs/overview.png)

## Architecture
![](/Docs/architecture.png)

## Dependencies
![](/Docs/dependencies.jpg)

## Project dependencies
![](/Docs/project-dependencies.jpg)

## Code flow
![](/Docs/flowchart.png)
![](/Docs/code-flow.jpg)

## Repository & Unit Of Work
![](/Docs/custom-repo-versus-db-context.png)

# Techical Stack
- ASP.NET Core 3.1 (with .NET Core 3.1)
- ASP.NET WebApi Core
- ASP.NET Identity Core
- Entity Framework Core 3.1
- .NET Core Native DI
- AutoMapper
- FluentValidator
- MediatR
- Swagger UI
- MSSQL
- xUnit
- Moq
- Fluent Assertions
- Polly

# Design Patterns
- Domain Driven Design
- Domain Events
- Domain Notification
- CQRS
- Event Sourcing
- Unit Of Work
- Repository & Generic Repository
- Inversion of Control / Dependency injection
- ORM
- Mediator
- Specification Pattern

# How to run
- Visual Studio: `Just run`
- VSCode: `Just run`
- Terminal: `dotnet run --project src/DDD.Services.Api/DDD.Services.Api.csproj --launch-profile Dev`

# Testing
- Terminal: `dotnet test`

# Docker

```sh
docker build -t aspnetcore-docker-image .
docker run -it --rm -p 3000:80 --name aspnetcore-docker-container aspnetcore-docker-image
docker run -d -p 3000:80 --name aspnetcore-docker-container aspnetcore-docker-image
```

- http://localhost:3000/

# Swagger (Dev env only)
- http://localhost:5000/swagger

# Health check (Staging & Prod env only)
- http://localhost:5000/healthchecks-ui

# TODO
- [x] Use multiple environments
- [x] Transaction (Unit of Work)
- [x] Validation (FluentValidation)
- [x] Response wrapper
- [x] Async/Await
- [x] REST
- [x] JWT
- [x] Mapping (AutoMapper)
- [x] API Specification, API Definition (Swagger)
- [x] ORM {Entity Framework Core}
- [x] Middleware
- [x] CORS
- [x] Pagination
- [x] Sorting
- [x] Error Handling, Global Exception
- [x] HealthCheck
- [x] Mail
- [x] Http
- [x] Database Auditing: CreatedAt/UpdatedAt CreatedBy/UpdatedBy
- [x] Soft Delete
- [x] Common: Constants, Helpers
- [x] Docker
- [x] EF: Shadow Properties
- [x] Events
- [x] Unit Testing
- [x] Integration Testing
- [x] Scoped over Transient
- [x] Use `abstract` keyword to appropriate class
- [x] Use `IQueryable`, `IEnumerable`, `IList` interfaces
- [ ] Migration, Scaffold
- [ ] Data Seeding
- [ ] Logging
- [ ] OAuth2
- [ ] SignalR
- [ ] Search
- [ ] Kafka, RabbitMQ
- [ ] Microservices, API Gateway
- [ ] Multi-tenancy
- [ ] StyleCop
- [ ] API Versioning
- [ ] API Versioning with Swagger
- [ ] Primary Key to Integer
- [ ] File storage: Upload/Download
- [ ] Kubernetes
- [ ] Globalization & Localization
- [ ] Caching
- [ ] Kestrel
- [ ] Secret Manager
- [ ] Task scheduling & Queues
- [ ] Session & Cookie
- [ ] Notifications
- [ ] Encryption & Hashing
- [ ] EF: No-tracking queries
- [ ] Dapper, Dapper Contrib
- [ ] BulkInsert, BulkUpdate, Async method for IRepository
- [ ] Use NetStandard 2.1 for Class Library

# References
- https://github.com/EduardoPires/EquinoxProject
- https://docs.microsoft.com/en-us/aspnet/core/security/authorization/roles?view=aspnetcore-3.1
- https://docs.microsoft.com/en-us/aspnet/core/security/authorization/claims?view=aspnetcore-3.1
- https://docs.microsoft.com/en-us/aspnet/core/security/authorization/policies?view=aspnetcore-3.1
- https://docs.microsoft.com/en-us/aspnet/core/security/authorization/limitingidentitybyscheme?view=aspnetcore-3.1
- https://www.red-gate.com/simple-talk/dotnet/c-programming/policy-based-authorization-in-asp-net-core-a-deep-dive/
- https://docs.microsoft.com/en-us/archive/msdn-magazine/2017/october/cutting-edge-policy-based-authorization-in-asp-net-core
- https://dev.azure.com/Techhowdy/_git/NG_Core_AuthRTDB
- https://github.com/Elfocrash/Youtube.AspNetCoreTutorial
- https://www.meziantou.net/entity-framework-core-soft-delete-using-query-filters.htm
- https://docs.microsoft.com/en-us/aspnet/core/fundamentals/environments
- https://michael-mckenna.com/multi-tenant-asp-dot-net-core-application-tenant-resolution
- https://stackify.com/writing-multitenant-asp-net-core-applications/
- https://github.com/DanielRBowen/SimpleMultiTenant
- https://deviq.com/specification-pattern/
