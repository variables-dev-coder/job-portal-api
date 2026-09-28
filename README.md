# Job Portal API

A production-oriented Job Portal REST API built with Java and Spring Boot.

This project provides backend APIs for candidates, recruiters, companies, jobs, applications, resumes, and role-based access control.

---

## 🚀 Project Overview

The Job Portal API is designed to simulate a real-world recruitment platform where:

- Candidates can create profiles and search for jobs.
- Candidates can save jobs and apply with their resumes.
- Recruiters can create and manage job postings.
- Recruiters can review applicants and update application status.
- Admins can manage users, companies, jobs, and applications.

---

## 🛠️ Tech Stack

- Java 17
- Spring Boot
- Spring Web
- Spring Data JPA
- MySQL
- Maven
- REST API
- Git & GitHub

---

## 👥 User Roles

### Candidate
- Register and login
- Manage profile
- Search and filter jobs
- Save jobs
- Upload resume
- Apply for jobs
- Track application status

### Recruiter
- Register and login
- Manage company profile
- Create job postings
- Update and close jobs
- View applicants
- Update application status

### Admin
- Manage users
- Manage companies
- Manage jobs
- Manage applications
- View platform statistics

---

## 📦 Core Modules

```text
Authentication
Candidate
Company
Job
Application
Resume
Saved Jobs
Admin
🏗️ Architecture
Client / Postman
       ↓
REST Controller
       ↓
Service Layer
       ↓
Repository Layer
       ↓
MySQL Database

The application follows a layered architecture to keep business logic, API handling, and database access separated.

🗄️ Core Entities
User
CandidateProfile
Company
Job
Application
Resume
SavedJob
Main Relationships
User
 ├── CandidateProfile
 └── Company

Company
 └── Jobs

Candidate
 ├── Resumes
 ├── Applications
 └── Saved Jobs

Job
 ├── Applications
 └── Saved Jobs
🔐 Security

Planned security features:

Spring Security
JWT Authentication
Role-Based Authorization
Password Hashing
API Validation
Global Exception Handling
📋 Application Workflow
Candidate Registration
        ↓
Login
        ↓
Create Profile
        ↓
Search Jobs
        ↓
Upload Resume
        ↓
Apply for Job
        ↓
Recruiter Reviews Application
        ↓
Under Review
        ↓
Shortlisted
        ↓
Interview
        ↓
Selected / Rejected
🔌 API Modules
Authentication
POST /api/auth/register
POST /api/auth/login
GET  /api/auth/me
Jobs
GET    /api/jobs
GET    /api/jobs/{id}
POST   /api/jobs
PUT    /api/jobs/{id}
DELETE /api/jobs/{id}
Applications
POST  /api/applications
GET   /api/applications/my
GET   /api/applications/{id}
PATCH /api/applications/{id}/status

API endpoints will evolve as the project development progresses.

▶️ How to Run
Prerequisites

Make sure the following are installed:

Java 17+
Maven
MySQL
Git
Clone Repository
git clone https://github.com/variables-dev-coder/job-portal-api.git
Navigate to Project
cd job-portal-api
Run the Application
./mvnw spring-boot:run

For Windows:

mvnw.cmd spring-boot:run
🧪 API Testing

Postman will be used for API development and testing.

Future API documentation will include:

Request examples
Response examples
Authentication details
Error responses
HTTP status codes
🔮 Future Enhancements
JWT Authentication
Spring Security
Resume File Upload
Advanced Job Search
Pagination & Sorting
Email Notifications
Redis Caching
Kafka Event Processing
Docker
AWS Deployment
CI/CD Pipeline
API Documentation with Swagger/OpenAPI
📌 Project Status

🚧 In Development

This project is being developed step-by-step with a focus on real-world backend development practices and production-oriented architecture.

👨‍💻 Author

Munna

Java Backend Developer | Spring Boot | REST APIs | Problem Solving

📄 License

This project is created for learning, portfolio, and demonstration purposes.


### তারপর

Save করো:

```text
Ctrl + S