# Go URL Shortener

Production-grade URL Shortener built with Go, PostgreSQL, Redis, JWT Authentication, Rate Limiting, Docker, CI/CD, and Analytics.

## Overview

Go URL Shortener is a backend service that converts long URLs into short, shareable links while providing authentication, analytics, caching, and rate limiting.

This project is designed to demonstrate production-level backend engineering practices using Golang.

---

## Features

### Core Features
- Create short URLs
- Custom short codes
- URL redirection
- URL expiration support

### Authentication & Security
- JWT Authentication
- User Registration & Login
- Password Hashing (bcrypt)
- Role-Based Access Control (RBAC)

### Performance
- Redis Caching
- Database Connection Pooling
- Optimized Redirect Handling

### Analytics
- Click Tracking
- Total Visits
- Creation Date
- Link Usage Statistics

### Reliability
- Structured Logging
- Error Handling
- Request Validation
- Health Check Endpoint

### DevOps
- Docker Support
- Docker Compose
- Environment Configuration
- GitHub Actions CI/CD

---

## Tech Stack

| Component | Technology |
|------------|------------|
| Language | Go |
| Web Framework | Gin |
| Database | PostgreSQL |
| Cache | Redis |
| Authentication | JWT |
| Containerization | Docker |
| CI/CD | GitHub Actions |
| Documentation | Swagger/OpenAPI |

---

## Project Structure

```text
go-url-shortener/
│
├── cmd/
│   └── server/
│
├── internal/
│   ├── handlers/
│   ├── services/
│   ├── repository/
│   ├── middleware/
│   ├── models/
│   └── config/
│
├── docs/
│
├── scripts/
│
├── tests/
│
├── docker/
│
├── .github/
│   └── workflows/
│
├── Dockerfile
├── docker-compose.yml
├── go.mod
├── go.sum
└── README.md
```

---

## API Endpoints

### Authentication

| Method | Endpoint |
|----------|----------|
| POST | /api/v1/auth/register |
| POST | /api/v1/auth/login |

### URL Management

| Method | Endpoint |
|----------|----------|
| POST | /api/v1/urls |
| GET | /api/v1/urls |
| GET | /api/v1/urls/:id |
| DELETE | /api/v1/urls/:id |

### Analytics

| Method | Endpoint |
|----------|----------|
| GET | /api/v1/analytics/:id |

### Health Check

| Method | Endpoint |
|----------|----------|
| GET | /health |

---

## Planned Features

- QR Code Generation
- Custom Domains
- Link Password Protection
- Geo Analytics
- User Dashboard
- Admin Dashboard
- Kubernetes Deployment
- Distributed Rate Limiting

---

## Getting Started

### Clone Repository

```bash
git clone https://github.com/your-username/go-url-shortener.git
cd go-url-shortener
```

### Run with Docker

```bash
docker-compose up --build
```

### Run Locally

```bash
go mod tidy
go run cmd/server/main.go
```

---

## Learning Objectives

This project demonstrates:

- REST API Development
- Clean Architecture
- Authentication & Authorization
- Caching with Redis
- Database Design
- Docker Deployment
- CI/CD Pipelines
- Production Backend Engineering

---

## License

This project is licensed under the MIT License.
