# ✅ Project Requirements - SkillUp Backend

## Functional Requirements

### 👤 User Management

- Register / Login / Logout (JWT)
- Email verification
- Password reset
- Role-based access: Student, Instructor, Admin

### 🎓 Learning Platform

- CRUD Courses, Lessons, Quizzes
- Enroll in courses (free or paid)
- Track lesson progress
- Submit quiz answers and get results

### 🧾 Payments

- Purchase paid courses using Stripe
- Webhook to confirm payment and enroll user

### 📁 File Handling

- Upload lesson materials (PDFs, videos, thumbnails)
- Switch between local storage and S3

### 📬 Notifications

- Email notifications on important events
- Scheduled reminders for unfinished courses

### 🛠️ Admin Dashboard (API layer only)

- Manage users, courses, and content
- View system analytics

---

## Non-Functional Requirements

- Secure by default (rate-limiting, input validation, hashed passwords)
- Modular DDD architecture
- Environment-based configuration
- Logs & error tracking
- API documentation (Swagger or similar)
- Unit tests
