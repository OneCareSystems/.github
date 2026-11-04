# OneCare – Clinic Integrated Pharmacy Management System

OneCare is a web-based Clinic Integrated Pharmacy Management System developed as part of the **SENG 34213 – System Development Project, University of Kelaniya**.

The system integrates clinic operations and pharmacy management, including patient registration, appointments, consultations, prescriptions, medicine dispensing, inventory management, billing, reporting, and an AI-powered chatbot.

---

## 1. Live Application

| Environment | URL |
|---|---|
| Live Application | http://3.27.171.160/ |
| Domain URL | http://one-care.tech |

---

## 2. GitHub Repositories

The OneCare project is organized into multiple repositories.

| Repository | Description |
|---|---|
| [Frontend](https://github.com/OneCareSystems/onecare-frontend) | React-based user interface |
| [Backend](https://github.com/OneCareSystems/onecare-backend) | Spring Boot REST API and business logic |
| [Chatbot](https://github.com/OneCareSystems/onecare-chatbot) | Django-based AI chatbot service |
| [Infrastructure](https://github.com/OneCareSystems/onecare-infra) | Docker Compose and deployment configuration |
| [Testing](https://github.com/OneCareSystems/onecare-testing) | API and integration testing resources |
| [Documentation](https://github.com/OneCareSystems/onecare-documents) | SRS, SDS, and project documentation |
| [GitHub Organization](https://github.com/OneCareSystems) | All OneCare repositories |

For detailed installation instructions, configurations, testing commands, and deployment information, refer to the README file in each repository.

---

## 3. System Architecture

OneCare follows a modular architecture where the frontend communicates with the backend REST API. The backend connects to the MySQL database, Redis, and the separate Django chatbot service.

```text
             Patients and Staff
                    |
                    v
             React Frontend
                    |
                    v
           Spring Boot Backend
             /      |       \
            v       v        v
          MySQL   Redis   Django Chatbot
                              |
                              v
                      Knowledge Base
                       and AI Retrieval
```

The chatbot operates as a separate service and communicates with the backend through protected service-to-service integration.

---

## 4. Main Features

### Public Patient Portal
- Patient registration and login
- Password reset
- Online appointment booking
- Clinic information
- English and Tamil language support
- Patient chatbot

### Super Admin Module
- Dashboard
- User management
- Role and access control
- Clinic configuration
- System maintenance
- Audit logs
- Reports

### Admin Module
- Patient registration and management
- Appointment management
- Queue management
- Billing
- Clinic reports
- Knowledge-base management

### Doctor Module
- Doctor dashboard
- Appointment schedules
- Patient records
- Consultations
- Clinical notes
- Prescription management

### Pharmacist Module
- Pharmacist dashboard
- Prescription dispensing queue
- Medicine inventory management
- Stock updates
- External dispensing
- Pharmacy reports

### AI Chatbot
- English and Tamil query support
- Knowledge-base-based responses
- Document and approved URL processing
- Semantic retrieval using Sentence Transformers and FAISS
- Medical safety guardrails

---

## 5. Technology Stack

| Component | Technologies |
|---|---|
| Frontend | React 19, Vite, Redux Toolkit, React Router, Tailwind CSS |
| Backend | Java 21, Spring Boot 3.5.x, Spring Security, Spring Data JPA |
| Database | MySQL 8.x |
| Cache | Redis |
| Chatbot | Python 3.11, Django 5.2, Django REST Framework |
| AI Retrieval | Sentence Transformers, FAISS |
| API Documentation | Swagger / OpenAPI |
| Frontend Testing | Vitest, React Testing Library, MSW, Playwright |
| Backend Testing | JUnit 5, Mockito, MockMvc, JaCoCo |
| DevOps | Docker, Docker Compose, GitHub Actions, Nginx |

---

## 6. Local Development

The infrastructure repository provides the coordinated setup for running the complete application.

**Basic steps:**

1. Clone the required repositories.
2. Install the prerequisites mentioned in each repository README.
3. Configure the required environment variables.
4. Follow the Docker Compose instructions in the [Infrastructure Repository](https://github.com/OneCareSystems/onecare-infra).
5. Start the application and access the frontend using the local URL.

### Default Local Service Ports

| Service | Port |
|---|---:|
| Frontend | 3000 |
| Backend | 8080 |
| Chatbot | 8000 |
| MySQL | 3306 |
| Redis | 6379 |

Refer to the Infrastructure README for the complete development and deployment setup.

---

## 7. Demo User Accounts

The following demo usernames are available for the corresponding staff roles.

| Role | Username | Password
| --- | --- | ----
| Pharmacist | `pharmacist1` | Passw0rd!2026
| Doctor | `Doctor kuruparan` | Passw0rd!2026
| Super Admin | `Superadmin` | Passw0rd!2026
| Admin | `Admin` | 


## 8. Security

- Role-based authentication and authorization
- JWT-based access and refresh tokens
- Password hashing
- Protected API endpoints
- Audit logging
- Redis-based token revocation
- Environment-based secret configuration
- Protected chatbot service integration

**Important:** Never commit passwords, database credentials, JWT secrets, chatbot service tokens, SMTP credentials, or other sensitive configuration values to GitHub.

---

## 9. Testing and CI/CD

The project uses automated testing and GitHub Actions workflows across its repositories.

- Frontend unit and component testing
- Frontend end-to-end testing with Playwright
- Backend unit and integration testing
- API testing
- Automated build and validation workflows

For current workflow results, visit the Actions tab of the relevant repository.

---

## 10. Project Information

| Item | Details |
|---|---|
| Project Name | OneCare – Clinic Integrated Pharmacy Management System |
| Course | SENG 34213 – System Development Project |
| Institution | University of Kelaniya |
| GitHub Organization | [OneCareSystems](https://github.com/OneCareSystems) |

---

**OneCare – Integrated Clinic and Pharmacy Management System**  
*Simplifying clinic operations and pharmacy management through technology.*
