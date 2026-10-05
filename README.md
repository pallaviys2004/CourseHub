# 🎓 CourseHub – Online Learning & Course Management Platform

CourseHub is a full-stack online learning platform developed using **Java, Spring Boot, Hibernate/JPA, MySQL, and HTML/CSS**. The application allows students to browse and enroll in courses, track their learning progress, attempt mock tests, submit reviews, receive certificates, and make course payments.

The system also provides administrative features for managing users, trainers, courses, categories, modules, lessons, tests, and certificates.

---

## 🚀 Features

### 👨‍🎓 Student Features
- User registration and login
- Browse available courses
- View course details
- Enroll in courses
- Track course and module progress
- Access course modules and lessons
- Attempt mock tests
- View mock test results
- Submit course reviews
- Generate/view course certificates
- Course payment integration using Razorpay

### 👨‍🏫 Trainer Features
- Manage trainer-related course content
- Manage course categories
- Create and manage courses
- Manage modules and lessons
- Track course-related information

### 👨‍💼 Admin Features
- Admin authentication
- Admin dashboard
- Manage users
- Manage students and trainers
- Manage courses
- Manage categories
- Manage modules and lessons
- Manage mock tests and questions
- Manage certificates
- Monitor course-related activities

### 💳 Payment
- Razorpay payment gateway integration
- Payment status management
- Store payment transaction details

### 🔐 Security
- Spring Security
- Role-based access control
- Custom user details service
- Protected application endpoints
- Unauthorized access handling

---

## 🛠️ Technologies Used

### Backend
- Java
- Spring Boot
- Spring MVC
- Spring Data JPA
- Hibernate
- Spring Security
- REST APIs

### Database
- MySQL

### Frontend
- HTML
- CSS
- Thymeleaf
- JavaScript

### Payment
- Razorpay

### Development Tools
- Eclipse / IntelliJ IDEA
- Maven
- Git & GitHub
- Postman

---

## 🏗️ Project Architecture

The project follows a layered architecture:

```text
CourseHub
│
├── Controller
│   ├── AdminDashboardController
│   ├── CourseController
│   ├── StudentController
│   ├── UserController
│   ├── EnrollmentController
│   ├── LessonController
│   ├── ModuleController
│   ├── MockTestController
│   ├── CertificateController
│   └── ReviewController
│
├── Service
│   └── Business Logic
│
├── Repository
│   └── Database Operations
│
├── Entity
│   ├── User
│   ├── Student
│   ├── Trainer
│   ├── Course
│   ├── Category
│   ├── Module
│   ├── Lesson
│   ├── Enrollment
│   ├── Certificate
│   ├── Review
│   ├── MockTest
│   └── Question
│
├── DTO
│   └── Request & Response Objects
│
├── Security
│   ├── SecurityConfig
│   └── CustomUserDetailsService
│
├── Exception
│   └── Global Exception Handling
│
├── Payment
│   ├── PaymentController
│   ├── PaymentService
│   ├── PaymentRepository
│   └── Payment Entity
│
└── Resources
    ├── templates
    ├── static
    └── application.properties


User
  │
  ▼
Registration / Login
  │
  ▼
Authentication & Authorization
  │
  ├───────────────┐
  ▼               ▼
Student          Admin/Trainer
  │               │
  ▼               ▼
Browse Courses   Manage Courses
  │               │
  ▼               ▼
Enroll           Manage Modules
  │               │
  ▼               ▼
Payment          Manage Lessons
  │
  ▼
Learn Course
  │
  ▼
Track Progress
  │
  ▼
Attempt Mock Test
  │
  ▼
Complete Course
  │
  ▼
Certificate
