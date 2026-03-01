
# Full Stack Cloud Authentication System

A production-ready full stack web application built with **Angular**, **FastAPI**, and **Google Cloud Platform**, implementing secure **JWT-based authentication**, scalable backend APIs, and cloud-native deployment.

This project demonstrates modern web application development aligned with real-world cloud engineering practices.

---

## Live Architecture

Frontend → Angular SPA  
Backend → FastAPI REST API  
Database → PostgreSQL  
Deployment → Docker, Google Cloud Run  

---

## Key Features

- Secure user registration and login
- JWT-based authentication and authorization
- Protected routes using Angular Guards
- Password hashing with bcrypt
- RESTful API architecture
- Cloud-ready containerized deployment
- Scalable backend using FastAPI

---

## Tech Stack

**Frontend**

- Angular
- TypeScript
- HTML
- CSS

**Backend**

- FastAPI
- Python
- JWT Authentication
- REST APIs

**Database**

- PostgreSQL

**Cloud & DevOps**

- Docker
- Google Cloud Platform (Cloud Run)
- GitHub Actions (CI/CD ready)

---

## Project Structure

```

angular-fastapi-cloud-auth-system
│
├── frontend
│   └── src
│       └── app
│           ├── pages
│           │   ├── login
│           │   │   ├── login.component.ts
│           │   │   ├── login.component.html
│           │   │   └── login.component.css
│           │   │
│           │   ├── register
│           │   │   ├── register.component.ts
│           │   │   ├── register.component.html
│           │   │   └── register.component.css
│           │   │
│           │   └── dashboard
│           │       ├── dashboard.component.ts
│           │       ├── dashboard.component.html
│           │       └── dashboard.component.css
│           │
│           ├── components
│           │   └── navbar
│           │       ├── navbar.component.ts
│           │       ├── navbar.component.html
│           │       └── navbar.component.css
│           │
│           └── services
│               └── auth.service.ts
│
├── backend
│   ├── main.py
│   ├── models.py
│   ├── database.py
│   └── auth.py
│
├── Dockerfile
│
└── README.md

`````

---

## Authentication Flow

1. User registers via Angular frontend  
2. Backend hashes password and stores user  
3. User logs in  
4. Backend generates JWT token  
5. Token used to access protected routes  

---

## API Endpoints

### Register

POST `/register`

````json
{
  "email": "user@gmail.com",
  "password": "password"
}
`````

---

### Login

POST `/login`

Response:

```json
{
  "access_token": "jwt_token"
}
```

---

### Protected Route

GET `/profile`

Requires JWT token.

---

## Local Setup

### Clone repository

```bash
git clone https://github.com/7amitesh/angular-fastapi-cloud-auth-system.git
```

---

### Backend Setup

```bash
cd backend

python -m venv venv

venv\Scripts\activate

pip install -r requirements.txt

uvicorn main:app --reload
```

Backend runs:

```
http://127.0.0.1:8000
```

---

### Frontend Setup

```bash
cd frontend

npm install

ng serve
```

Frontend runs:

```
http://localhost:4200
```

---

## Docker Deployment

Build container:

```bash
docker build -t auth-system .
```

Run container:

```bash
docker run -p 8000:8000 auth-system
```

---

## Google Cloud Deployment

Deploy to Cloud Run:

```bash
gcloud run deploy
```

Supports:

* Auto scaling
* Container deployment
* Production workloads

---

## Security Implementation

* Password hashing using bcrypt
* JWT authentication
* Secure API routes
* Token validation

---

## Engineering Highlights

* Cloud-native architecture
* Scalable REST API backend
* Secure authentication system
* Containerized deployment
* Production-ready design

---

## Author

**Amitesh Kumar**

GitHub
[https://github.com/7amitesh](https://github.com/7amitesh)

LinkedIn
[https://linkedin.com/in/amitesh-k](https://linkedin.com/in/amitesh-k)

---

## Purpose

This project demonstrates practical experience with:

* Angular web application development
* FastAPI backend engineering
* Authentication and authorization
* Google Cloud deployment
* Cloud-native software architecture

```
cture Google recruiters expect in 2026** that increases shortlist chances significantly.
```
