# Task-Management-System

A modern full-stack task management application built with **FastAPI**, **SQLAlchemy**, **SQLite**, and **JWT Authentication**. The system enables users to securely manage daily tasks, track progress, prioritize work, and monitor productivity through a clean dashboard and RESTful APIs.

---

## Overview

Task-Management-System is designed to help users organize and manage tasks efficiently. The application provides secure authentication, task tracking, filtering, analytics, and user-specific data management.

The project demonstrates backend engineering concepts such as API development, database modeling, authentication, authorization, data validation, and productivity-focused application design.

---

## Features

### Authentication & Security

* User Registration
* Secure Login System
* JWT Authentication
* OAuth2 Integration
* Password Hashing with Bcrypt
* Protected API Routes

### Task Management

* Create Tasks
* Update Tasks
* Delete Tasks
* View Individual Tasks
* Manage Task Status
* Priority Assignment (Low, Medium, High)

### Productivity Features

* Task Completion Tracking
* Progress Monitoring
* Task Search Functionality
* Advanced Filtering
* Pagination Support
* User-Specific Task Management

### Analytics

* Total Tasks Count
* Completed Tasks Count
* Pending Tasks Count
* In-Progress Tasks Count
* Completion Rate Calculation

---

## Tech Stack

| Category       | Technologies          |
| -------------- | --------------------- |
| Backend        | FastAPI               |
| Database       | SQLite                |
| ORM            | SQLAlchemy            |
| Authentication | JWT, OAuth2           |
| Validation     | Pydantic              |
| Security       | Passlib (Bcrypt)      |
| Frontend       | HTML, CSS, JavaScript |
| Templates      | Jinja2                |
| Server         | Uvicorn               |

---

## Project Structure

```text
Task-Management-System/
│
├── static/
│   ├── css/
│   ├── js/
│   └── assets/
│
├── templates/
│   └── dashboard.html
│
├── main.py
├── README.md
├── pyproject.toml
└── uv.lock
```

---

## Database Schema

### User

| Field      | Type     |
| ---------- | -------- |
| id         | Integer  |
| username   | String   |
| password   | String   |
| created_at | DateTime |

### Task

| Field       | Type     |
| ----------- | -------- |
| id          | Integer  |
| title       | String   |
| description | String   |
| status      | String   |
| priority    | String   |
| completed   | Boolean  |
| created_at  | DateTime |
| updated_at  | DateTime |
| user_id     | Integer  |

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/Task-Management-System.git

cd Task-Management-System
```

### Create Virtual Environment

```bash
python -m venv .venv
```

Activate:

**Windows**

```bash
.venv\Scripts\activate
```

**Linux / Mac**

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

or

```bash
pip install fastapi uvicorn sqlalchemy python-jose passlib bcrypt jinja2 python-multipart
```

---

## Running the Application

Start the FastAPI server:

```bash
python main.py
```

or

```bash
uvicorn main:app --reload
```

Open your browser:

```text
http://localhost:8000
```

---

## API Endpoints

### Authentication

| Method | Endpoint  | Description                |
| ------ | --------- | -------------------------- |
| POST   | /register | Register User              |
| POST   | /token    | Login & Generate JWT Token |

### Tasks

| Method | Endpoint             |
| ------ | -------------------- |
| POST   | /tasks/              |
| GET    | /tasks/              |
| GET    | /tasks/{id}          |
| PUT    | /tasks/{id}          |
| DELETE | /tasks/{id}          |
| GET    | /tasks/stats/summary |

---

## Sample Workflow

1. Register a new account.
2. Login and receive JWT access token.
3. Create new tasks.
4. Update task status and priority.
5. Search and filter tasks.
6. Track completion progress.
7. View productivity statistics.

---

## Key Learning Outcomes

* FastAPI Application Development
* REST API Design
* JWT Authentication
* OAuth2 Security
* Database Modeling
* SQLAlchemy ORM
* User Authorization
* CRUD Operations
* Backend Architecture
* API Validation
* Secure Web Development

---

## Future Enhancements

* Role-Based Access Control (RBAC)
* Email Notifications
* Task Reminders
* Calendar Integration
* Dark Mode UI
* Team Collaboration Features
* Docker Deployment
* PostgreSQL Support
* Real-Time Updates with WebSockets
* Cloud Deployment

---

## Author

**Mahor Binish**

Artificial Intelligence & Machine Learning Student

Oracle Certified Generative AI Professional

GitHub: [https://github.com/M-Binish](https://github.com/M-Binish)

LinkedIn: [https://www.linkedin.com/in/mahor-binish-070572324](https://www.linkedin.com/in/mahor-binish-070572324)

---

## License

This project is licensed under the MIT License.

Feel free to fork, improve, and build upon this project.
