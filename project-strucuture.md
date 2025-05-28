# 🏗️ Project Structure - SkillUp (DDD Oriented)

## Root

```
/SkillUp
├── /src
│    ├── SkillUp.API # HTTP layer
│    ├── SkillUp.Application # Use cases, DTOs, validators
│    ├── SkillUp.Domain # Core domain models, interfaces, value objects
│    ├── SkillUp.Infrastructure # Data access, file/email/payment services
│    └── SkillUp.BackgroundJobs # Scheduled/queued tasks
├── /tests
│    ├── SkillUp.UnitTests
│    └── SkillUp.IntegrationTests
├── docker-compose.yml
└── README.md
```

## Domain Layer (`SkillUp.Domain`)

- `Entities/` → `User.cs`, `Course.cs`, `Lesson.cs`
- `ValueObjects/` → `Email.cs`, `Price.cs`
- `Enums/` → roles, lesson types, payment statuses
- `Events/` → domain events (e.g., `CoursePurchased`)
- `Interfaces/` → abstract contracts (`ICourseRepository`, `IStorageService`)

## Application Layer (`SkillUp.Application`)

- `DTOs/` → Input/output objects
- `Interfaces/` → Application-level services
- `Services/` → Orchestrate domain logic
- `Validators/` → FluentValidation or custom

## Infrastructure Layer (`SkillUp.Infrastructure`)

- `Persistence/` → EF Core DbContext, config
- `Repositories/` → Concrete EF implementations
- `Storage/` → NGINX local or Amazon S3
- `Email/` → MailKit integration
- `Stripe/` → Payment service

## API Layer (`SkillUp.API`)

- `Controllers/` → HTTP endpoints
- `Middleware/` → JWT, exception handling, logging
- `Configuration/` → Service and pipeline setup

## Background Jobs (`SkillUp.BackgroundJobs`)

- `Workers/` → Hosted services
- `QuartzJobs/` → Scheduled tasks (e.g., reminders)
