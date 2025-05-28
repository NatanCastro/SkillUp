# ✅ Project Requirements - SkillUp Backend (Progress Checklist)

## 👤 User Management

- [ ] User registration with email verification
- [ ] Login with JWT access + refresh tokens
- [ ] Logout and refresh token revocation
- [ ] Password reset via email
- [ ] Role-based access control (`Student`, `Instructor`, `Admin`)

## 🎓 Learning Platform

- [ ] Create/read/update/delete Courses
- [ ] Create/read/update/delete Lessons
- [ ] Create/read/update/delete Quizzes
- [ ] Enroll in free courses
- [ ] Enroll in paid courses (after Stripe payment)
- [ ] Track lesson and quiz progress
- [ ] Evaluate quiz submissions

## 💳 Payment System (Stripe)

- [ ] Integrate Stripe checkout session for paid courses
- [ ] Webhook for successful payment → auto-enrollment
- [ ] Handle failed and canceled payments

## 📁 File Handling

- [ ] Upload PDFs, videos, and thumbnails
- [ ] Serve files via local NGINX server (dev/testing)
- [ ] Switch to Amazon S3 for production

## 📬 Email Notifications

- [ ] Send registration and verification emails
- [ ] Send password reset emails
- [ ] Notify user of new course/lesson availability
- [ ] Schedule reminder emails (e.g., incomplete courses)

## 🛠️ Admin Dashboard (API endpoints)

- [ ] List/search users
- [ ] Manage courses and lessons
- [ ] View course enrollment analytics
- [ ] View quiz performance analytics

## 🔒 Security & Validation

- [ ] Passwords hashed with bcrypt
- [ ] Input validation (DTOs or FluentValidation)
- [ ] JWT token expiration & renewal logic
- [ ] Rate limiting or brute-force protection

## ⚙️ Non-Functional Requirements

- [ ] Docker Compose dev setup (Postgres, Redis, NGINX, MailHog)
- [ ] Environment-based configuration
- [ ] Centralized error handling & logging
- [ ] API documentation (Swagger/OpenAPI)
