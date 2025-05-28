# 📦 Tech Stack - SkillUp Backend

## 🖥️ Language & Framework

- **C#** (.NET 8)
- ASP.NET Core Web API

## 🗄️ Database

- **PostgreSQL**
  - Relational modeling for entities like courses, users, enrollments, etc.

## ⚡ Caching & Messaging

- **Redis**
  - Used for caching and optional pub/sub

## 🔐 Authentication & Security

- **JWT** (access + refresh tokens)
- Policy-based authorization
- BCrypt for password hashing

## 📧 Email

- **MailKit**
  - Used for registration, password reset, and notifications

## 💾 File Storage

- **Custom NGINX-based local storage** for dev/testing
- **Amazon S3** for production deployment

## 💳 Payments

- **Stripe API**
  - Course enrollment and payment webhook integration

## 🔧 Miscellaneous

- **Docker Compose** for local development
  - Services: Postgres, Redis, NGINX, MailHog
