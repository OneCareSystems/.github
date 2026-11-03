# 🏥 OneCare Systems

### Integrated Clinic & Pharmacy Management System

**Building smarter healthcare workflows through reliable software engineering.**

OneCare Systems is a software engineering project focused on developing an integrated clinic and pharmacy management platform. The system aims to streamline patient management, appointments, consultations, prescriptions, billing, and pharmacy operations through a centralized application.

Our goal is to improve operational efficiency, data consistency, and maintainability by applying software engineering best practices and modern technologies.

---

## 🎯 Project Objectives

- 👤 **Patient Management** — Maintain and manage patient information.
- 📅 **Appointment & Queue Management** — Organize appointments and patient flow.
- 🩺 **Clinical Management** — Support consultations and prescription workflows.
- 💊 **Pharmacy Management** — Manage medicines, dispensing, and external prescriptions.
- 💳 **Billing & Invoicing** — Support consultation billing and payment processing.
- 🔐 **Security & Access Control** — Enforce authentication and role-based permissions.
- 📊 **Auditability** — Maintain accountability through audit logging.
- ⚙️ **Reliable Infrastructure** — Support consistent development and deployment workflows.

## 🛠️ Technology Stack

| Area | Technologies |
|---|---|
| Frontend | React, Tailwind CSS |
| Backend API | Java, Spring Boot |
| Chatbot Service | Python, FastAPI |
| Database | MySQL |
| Caching | Redis |
| Authentication | Spring Security, JWT |
| Testing | JUnit, Vitest, Python testing tools |
| Infrastructure | Docker, Docker Compose |
| CI/CD | GitHub Actions |
| API Documentation | Swagger / OpenAPI |

## 🏗️ System Architecture

OneCare follows a modular architecture in which the React frontend communicates with the Spring Boot backend through REST APIs. The backend manages core business logic, authentication, authorization, and database operations. The Python chatbot operates as a separate service accessed through the backend API.

```text
             ┌──────────────────────┐
             │    React Frontend    │
             └──────────┬───────────┘
                        │ REST API
             ┌──────────▼───────────┐
             │   Spring Boot API    │
             └───┬────────┬─────┬───┘
                 │        │     │
          ┌──────▼───┐ ┌──▼───┐ ┌▼────────────────┐
          │  MySQL   │ │Redis │ │ Python Chatbot  │
          │ Database │ │Cache │ │ Service         │
          └──────────┘ └──────┘ │ (FastAPI)       │
                                └─────────────────┘
```

*This diagram illustrates the logical architecture. Actual service connections depend on the deployed configuration.*

## 📂 Repositories

Explore the OneCareSystems repositories:

- **[onecare-backend](https://github.com/OneCareSystems/onecare-backend)** — Spring Boot REST APIs, business logic, authentication, authorization, and data management.
- **[onecare-frontend](https://github.com/OneCareSystems/onecare-frontend)** — React-based user interface for clinic and pharmacy workflows.
- **[onecare-chatbot](https://github.com/OneCareSystems/onecare-chatbot)** — Python-based chatbot service supporting conversational assistance and knowledge-base functionality.
- **[All Organization Repositories](https://github.com/orgs/OneCareSystems/repositories)** — Explore the organization's available repositories and project modules.

## 🔒 Engineering Practices

We emphasize maintainable, secure, and testable software through:

- Feature-based development and issue tracking.
- Pull requests and peer code reviews.
- Protected branches and consistent branch naming.
- Automated builds, linting, and testing through CI.
- API validation and centralized error handling.
- Role-based authorization and secure credential management.
- Docker-based development environments.
- Technical documentation and continuous improvement.

## 👥 Team & Collaboration

OneCare Systems is developed collaboratively as part of a software engineering project at the University of Kelaniya.

We value clear communication, shared ownership, constructive code reviews, and continuous learning throughout the software development lifecycle.

## 🚀 Project Status

**Status:** Under active development.

Features, integrations, testing, and deployment configurations evolve as implementation progresses.
