# 🎓 SkillUp - Backend API

SkillUp is a scalable and modular backend system for an online learning platform. It supports user management, course content, lesson tracking, payments, and file uploads. Built with a Domain-Driven Design (DDD) architecture, it integrates robust components like Redis, Stripe, MailKit, and Amazon S3.

---

## 📚 Documentation

- 🧱 [Tech Stack](./tech-stack.md)
- ✅ [Feature Checklist](./project-requirements.md)
- 🗂️ [Project Structure](./project-structure.md)
- 📊 [Project Progress](./project-progress.md)

---

## 🚀 Features Overview

- 🔐 JWT-based authentication (access + refresh tokens)
- 🎓 Course creation, enrollment, progress tracking
- 💳 Stripe payments integration for paid courses
- 📁 File upload (local or S3)
- 📬 Email support via MailKit
- 🧠 DDD architecture with clear boundaries
- 🐳 Docker-ready dev environment

---

## 🧰 Tech Stack Highlights

- **Backend**: C# (.NET 8), ASP.NET Core
- **Database**: PostgreSQL
- **Cache/Queue**: Redis
- **Auth**: JWT (access + refresh)
- **Email**: MailKit
- **Payments**: Stripe
- **Storage**: Local (NGINX) → Amazon S3
- **Dev Tools**: Docker Compose, Swagger

---

## 🛠️ Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/)
- [Docker & Docker Compose](https://docs.docker.com/)
- PostgreSQL, Redis, MailHog, and NGINX configured via `docker-compose.yml`

### Run Locally

```bash
# Build and run backend with Docker dependencies
docker-compose up -d
dotnet build
dotnet run --project ./src/SkillUp.API
```

### Run Tests

```bash
# Run unit tests
dotnet test ./tests/SkillUp.UnitTests
dotnet test ./tests/SkillUp.IntegrationTests
```

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
