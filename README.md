# 🎓 Student Management System

A secure and scalable Student Management System built with FastAPI, implementing JWT Authentication, Role-Based Authorization, Redis Caching, Logging & Monitoring, and Comprehensive API Testing.

---

## 📌 Project Overview

This project provides a backend system for managing university students with secure authentication and role-based access control.

The system allows administrators to manage student records while students can view and update their own profiles.

---

## 🚀 Features

### Authentication & Security

- User Registration
- User Login
- JWT Token Generation
- JWT Token Validation
- Password Hashing
- Protected Routes

### Role-Based Authorization

#### Admin

- Create Students
- View Students
- Update Students
- Delete Students
- Access All Student Records

#### Student

- View Own Profile
- Update Limited Profile Information

---

### Student Management

- Create Student
- Retrieve All Students
- Retrieve Student By ID
- Update Student Information
- Delete Student
- Pagination Support
- Filtering Support

Examples:

- Filter by Department
- Filter by GPA

---

### Redis Caching

- Cache GET All Students
- Cache GET Student By ID
- Cache Invalidation After:
  - Create
  - Update
  - Delete

---

### Logging

The application logs:

- Incoming Requests
- Response Status Codes
- Response Time
- Authentication Events
- CRUD Operations
- Errors and Exceptions

---

### Monitoring Dashboard

Dashboard displays:

- API Request Count
- Response Time
- Error Rate
- System Health Status

Possible Technologies:

- Prometheus
- Grafana

---

### API Testing

Implemented using:

- Pytest
- FastAPI TestClient

Tests cover:

- Authentication
- Authorization
- CRUD Operations
- Validation Errors
- Edge Cases
- Protected Endpoints

---

## 🛠️ Tech Stack

### Backend

- FastAPI
- Python
- SQLAlchemy
- PostgreSQL / MySQL
- Pydantic

### Authentication

- JWT
- Passlib

### Caching

- Redis

### Monitoring

- Prometheus
- Grafana

### Testing

- Pytest
- TestClient

### Version Control

- Git
- GitHub

---

## 📂 Project Structure

```bash
student-management-system-fastapi/
│
├── app/
│   ├── main.py
│   │
│   ├── routes/
│   │   ├── auth.py
│   │   └── students.py
│   │
│   ├── models/
│   │   ├── user.py
│   │   └── student.py
│   │
│   ├── schemas/
│   │   ├── auth.py
│   │   └── student.py
│   │
│   ├── services/
│   │   ├── auth_service.py
│   │   └── student_service.py
│   │
│   ├── core/
│   │   ├── config.py
│   │   ├── security.py
│   │   └── roles.py
│   │
│   ├── database/
│   │   ├── connection.py
│   │   └── base.py
│   │
│   └── cache/
│       └── redis.py
│
├── tests/
│   ├── test_auth.py
│   ├── test_students.py
│   └── test_roles.py
│
├── logs/
│
├── requirements.txt
│
├── .env
│
└── README.md
```

---

## 🔑 API Endpoints

### Authentication

| Method | Endpoint | Description |
|----------|-----------|------------|
| POST | /auth/register | Register User |
| POST | /auth/login | Login User |

---

### Students

| Method | Endpoint |
|----------|-----------|
| GET | /students |
| GET | /students/{id} |
| POST | /students |
| PUT | /students/{id} |
| DELETE | /students/{id} |

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/your-username/student-management-system-fastapi.git
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

```bash
venv\Scripts\activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Application

```bash
uvicorn app.main:app --reload
```

---

## 🧪 Run Tests

```bash
pytest
```

---

## 📊 Monitoring

Prometheus collects:

- Request Count
- Response Time
- Error Rate

Grafana visualizes metrics through dashboards.

---

## 👥 Team Members

| Name | Role |
|--------|--------|
| Member 1 | Backend |
| Member 2 | Authentication |
| Member 3 | Authorization |
| Member 4 | Caching |
| Member 5 | Testing & Monitoring |

---

## 📄 License

This project is developed for educational purposes as part of the Backend Development with FastAPI course.
