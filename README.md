# Spring Security Web Demo

![Java](https://img.shields.io/badge/Java-25-orange?style=for-the-badge&logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-6DB33F?style=for-the-badge&logo=springboot)
![Spring Security](https://img.shields.io/badge/Spring_Security-6.x-6DB33F?style=for-the-badge&logo=springsecurity)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-3.x-005F0F?style=for-the-badge&logo=thymeleaf)
![Maven](https://img.shields.io/badge/Maven-3.9-C71A36?style=for-the-badge&logo=apachemaven)
![Docker](https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker)
![Render](https://img.shields.io/badge/Render-Deployed-46E3B7?style=for-the-badge&logo=render)

A production-ready Spring Boot application demonstrating authentication and authorization using **Spring Security**, **Thymeleaf**, **Docker**, and **Render**. This project showcases secure web application development with custom login, protected routes, Docker containerization, and cloud deployment.

---

# 🌐 Live Demo

🔗 **Application:** https://spring-security-web-demo.onrender.com

---

# ✨ Features

- Secure authentication using Spring Security
- Custom login page with Thymeleaf
- Public and protected routes
- User logout functionality
- In-memory authentication
- Embedded Tomcat Server
- Dockerized application
- Cloud deployment on Render
- Maven build automation
- Clean MVC architecture

---

# 🛠 Tech Stack

| Technology | Purpose |
|------------|---------|
| Java 25 | Programming Language |
| Spring Boot | Backend Framework |
| Spring Security | Authentication & Authorization |
| Spring MVC | Web Framework |
| Thymeleaf | Server-side Template Engine |
| Maven | Dependency Management |
| Docker | Containerization |
| Render | Cloud Deployment |
| Git | Version Control |
| GitHub | Source Code Hosting |

---

# 📁 Project Structure

```text
spring-security-web-demo
│
├── src
│   ├── main
│   │   ├── java
│   │   │   └── securing_web
│   │   │       ├── SecuringWebApplication.java
│   │   │       │
│   │   │       └── config
│   │   │           ├── MvcConfig.java
│   │   │           └── SecurityConfig.java
│   │   │
│   │   └── resources
│   │       ├── templates
│   │       │   ├── home.html
│   │       │   ├── login.html
│   │       │   └── hello.html
│   │       │
│   │       └── application.properties
│   │
│   └── test
│
├── Dockerfile
├── mvnw
├── mvnw.cmd
├── pom.xml
├── README.md
└── .gitignore
```

---

# 🏗 Architecture

```text
                     Browser
                        │
                        ▼
            Spring Boot Application
                        │
                        ▼
          Spring Security Filter Chain
               │                  │
               │                  │
               ▼                  ▼
        Public Route       Protected Route
          (Home)               (/hello)
               │                  │
               ▼                  ▼
          home.html        Login Required
                                   │
                                   ▼
                         Authentication
                                   │
                                   ▼
                             hello.html
```

---

# 🔐 Authentication Flow

```text
User
 │
 ▼
Home Page (/)
 │
 ▼
Protected Route (/hello)
 │
 ▼
Spring Security
 │
 ├── Authenticated? ───► YES ─────────► hello.html
 │
 └──────── NO
             │
             ▼
        Custom Login Page
             │
             ▼
      Username & Password
             │
             ▼
      Authentication Success
             │
             ▼
          hello.html
```

---

# 🚀 Getting Started

## Clone Repository

```bash
git clone https://github.com/khushimishra3112/spring-security-web-demo.git
```

## Navigate to Project

```bash
cd spring-security-web-demo
```

## Build Project

```bash
./mvnw clean package
```

## Run Application

```bash
./mvnw spring-boot:run
```

Open:

```
http://localhost:8080
```

---

# 🐳 Docker

## Build Docker Image

```bash
docker build -t spring-security-web-demo .
```

## Run Docker Container

```bash
docker run -d -p 8080:8080 --name spring-security-demo spring-security-web-demo
```

Open:

```
http://localhost:8080
```

---

# ☁️ Cloud Deployment

This application is deployed on **Render** using a Docker image hosted on **Docker Hub**.

Deployment Pipeline:

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
Docker Image
    │
    ▼
Docker Hub
    │
    ▼
Render
    │
    ▼
Live Application
```

---

# 🔑 Default Login Credentials

| Username | Password |
|----------|----------|
| user | password |

---

# 📚 Concepts Demonstrated

- Spring Boot Application Development
- Spring MVC
- Spring Security
- Authentication
- Authorization
- SecurityFilterChain
- Thymeleaf Templates
- Custom Login Page
- Logout Handling
- Embedded Tomcat
- Docker Containerization
- Cloud Deployment
- Git & GitHub Workflow

---

# 🎯 Learning Outcomes

Through this project, I learned how to:

- Build secure web applications with Spring Boot
- Configure authentication and authorization using Spring Security
- Develop dynamic web pages with Thymeleaf
- Protect application routes
- Containerize applications using Docker
- Deploy Spring Boot applications to the cloud
- Manage projects using Git and GitHub

---

# 🔮 Future Improvements

- MySQL Integration
- Spring Data JPA
- BCrypt Password Encryption
- User Registration
- Role-Based Access Control
- JWT Authentication
- REST API Development
- Unit & Integration Testing
- GitHub Actions CI/CD
- Kubernetes Deployment

---

# 👩‍💻 Author

**Khushi Mishra**

B.Tech Computer Science Engineering

GitHub: https://github.com/khushimishra3112

LinkedIn: https://www.linkedin.com/in/khushi-mishra-428091312/

---

# 📄 License

This project is licensed under the **MIT License**.

---

⭐ If you found this project helpful, consider giving it a star on GitHub.