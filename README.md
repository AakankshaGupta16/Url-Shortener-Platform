# 🔗 URL Shortener & Analytics Platform (Bitly Clone)

A high-performance, full-stack **URL Shortener & Analytics Platform** inspired by Bitly, built using **Spring Boot** and **React**. This application allows users to generate unique short URLs, manage them through a secure dashboard, and track real-time analytics such as click counts and usage trends.

---

## 🚀 Features

* **Secure Authentication**: Full signup and login flow using **JWT (JSON Web Tokens)** and Spring Security.
* **Link Management**: Generate, view, and manage shortened URLs linked to your account.
* **Real-time Analytics**: Track total click counts and monitoring usage patterns for every link.
* **Smart Redirection**: Efficient path-based routing that redirects users to the original destination instantly.
* **Secure Routing**: Implementation of protected frontend routes and authenticated backend API endpoints.
* **Dockerized Deployment**: Backend is containerized using multi-stage builds for easy scaling.

---

## 🛠 Tech Stack

### Backend
- **Framework**: Spring Boot 3.x
- **Security**: Spring Security, JWT
- **Data**: Spring Data JPA, PostgreSQL / MySQL
- **Build Tool**: Maven
- **Utilities**: Lombok, Docker

### Frontend
- **Library**: React.js
- **Styling**: Tailwind CSS
- **State Management**: Context API
- **API Client**: Axios

---

## 📂 Project Structure

```text
Url-Shortener-Platform/
├── url-shortener-sb/        # Spring Boot Backend
│   ├── src/                 # Application source code
│   ├── pom.xml              # Maven configuration
│   └── Dockerfile           # Backend containerization
│
├── url-shortener-react/     # React Frontend
│   ├── src/                 # Components, Context, and Services
│   └── package.json         # Frontend dependencies
│
└── README.md                # Documentation
---
```
## 🔐 Authentication Flow

- Users register and log in using email and password
- On successful login, a **JWT token** is issued
- Token is stored and used for authenticated API requests
- Protected routes are secured using Spring Security filters

---

## 📊 Analytics

- Track total clicks for each shortened URL
- Fetch analytics per URL and per user
- Dashboard view for managing URLs
- Backend optimized for fast redirection

---

## 🐳 Docker & Deployment

- Backend is dockerized using a multi-stage Dockerfile
- Cloud database setup supported
- Frontend and backend can be deployed independently
- Domain linking and routing supported

---

## ▶️ Running Locally

### Backend

```bash
cd url-shortener-sb
mvn spring-boot:run
```
### Frontend
```bash
cd url-shortener-react
npm install
npm start
```
🎯 Learning Outcomes

-Implemented JWT-based authentication in Spring Boot
-Built secure REST APIs with role-based access
-Integrated frontend and backend using REST APIs
-Designed analytics-driven features
-Dockerized a production-ready backend
-Understood real-world URL routing and redirection strategies

📌 Future Improvements
-Rate limiting for URL creation
-Expiry dates for short URLs
-Redis caching for faster redirects
-Advanced analytics dashboards
-Custom domain support per user
