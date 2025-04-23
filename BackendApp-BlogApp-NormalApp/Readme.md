# BlogApp - Scalable Blog Platform

## Project Overview
BlogApp is a full-stack, scalable blog application developed using Java Spring Boot and React. It allows users to create, manage, and view blog posts through a seamless and responsive interface. The application emphasizes performance, scalability, and a smooth user experience.

---

## Features
- **User Authentication:**
  - Email and password-based login system.
  - Only authenticated users can create blog posts.

- **Blog Management:**
  - Create, update, delete blogs (authenticated users).
  - View all blogs publicly.
  - Each blog includes a title, content, and timestamp.

- **Public Blog Listing:**
  - Paginated view of all published blogs.
  - Accessible to both authenticated and unauthenticated users.

- **Content Moderation:**
  - Admins can review and approve posts before publishing.

- **Responsive Design:**
  - Works across devices with mobile-first design.

- **Performance Optimization:**
  - Lazy loading and code splitting via `React.lazy` and `Suspense`.

- **Deployment:**
  - Containerized using Docker.
  - Deployed on Amazon EKS (Elastic Kubernetes Service) for scalability and high availability.

---

## Tech Stack
- **Backend:** Java, Spring Boot, Spring Data JPA, REST APIs
- **Frontend:** React, React Router, Redux, React Hooks, MUI (Material UI)
- **Database:** SQL-based (MySQL/PostgreSQL)
- **DevOps/Deployment:** Docker, Amazon EKS

---

## Loom Video Walkthrough
Watch a full walkthrough of the project here:
[Project Demo - Loom](https://www.loom.com/share/dcf16c48cf454859aa043e6be686fd29)

---

## Getting Started

### Prerequisites
- Java 17+
- Node.js (v18+ recommended)
- Docker (for deployment)
- MySQL/PostgreSQL database

---

### Backend Setup (Spring Boot)
```bash
cd blogapp-backend
./mvnw spring-boot:run
```
- Configure database in `application.properties`:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/blogapp
spring.datasource.username=root
spring.datasource.password=yourpassword
```

---

### Frontend Setup (React + MUI)
```bash
cd blogapp-frontend
npm install
npm run dev
```
- Make sure the frontend connects to backend API endpoints correctly (`http://localhost:8080` by default).

---

### Docker Deployment
Build and run using Docker Compose:
```bash
docker-compose up --build
```

---

## Folder Structure
```
blogapp/
├── blogapp-backend/       # Spring Boot API
├── blogapp-frontend/      # React frontend
├── docker-compose.yml     # Container orchestration
└── README.md
```

---

## Contribution
Feel free to fork the repo, create issues, and submit pull requests for improvements.

---

## License
MIT License

