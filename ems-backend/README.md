# Employee Management System

A full-stack Employee Management System with a **Spring Boot** backend and **React** frontend, containerized using **Docker** for easy setup and deployment.  

---

## 📌 Features  
- Employee data management (CRUD operations)  
- REST API powered by Spring Boot  
- React-based frontend with Vite  
- MySQL database integration  
- Containerized using Docker and Docker Compose  

---

## 🛠 Prerequisites  
Ensure you have the following installed:  
- [Docker](https://docs.docker.com/get-docker/)  
- [Docker Compose](https://docs.docker.com/compose/install/)  

---

## 🚀 Getting Started  

### 1️⃣ Clone the Repository  

```sh
git clone https://github.com/Aratrik123/Employee_management_system.git
cd Employee_management_system
```

### 2️⃣ Run the Project using Docker Compose

```sh
docker-compose up --build
```

This will start:

- MySQL database
- Backend (Spring Boot)
- Frontend (React)

### 3️⃣ Access the Application

- Frontend: http://localhost:3000
- Backend: http://localhost:8082
- MySQL Database: localhost:3306 (user: root, password: system)

### 4️⃣ Stopping the Application

```sh
docker-compose down
```

---

## 🏗 Project Structure

```
employee-management-system/
│── ems-backend/        # Spring Boot backend
│── ems-frontend/       # React frontend
│── docker-compose.yml  # Docker Compose configuration
│── README.md           # Project documentation
```

---
