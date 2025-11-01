# EventsApplication-Microservices-ReactJs
Parent repo with links to microservices and frontend for Event Management.

A complete **microservices-based web application** built using **Spring Boot**, **React.js**, and **PostgreSQL**, designed to manage cultural fest events, registrations, food stalls, and payments.  
This project demonstrates scalable architecture, modular microservices, and seamless integration between backend and frontend.

---

## 🧩 Microservices Architecture

```
[ React Frontend ] ⇄ [ API Gateway ] ⇄ [ Microservices ] ⇄ [ PostgreSQL Databases ]
```

### 📦 Microservices Included

| Service | Description | GitHub Link |
|----------|-------------|--------------|
| **Admin Service** | Manages admin login and event approval | [View Repo](https://github.com/arvind20222/EventsApplication-AdminService-) |
| **User Service** | Handles user registration and authentication | [View Repo](https://github.com/arvind20222/EventsApplication-UserService) |
| **Event Service** | Manages event CRUD operations | [View Repo](https://github.com/arvind20222/EventsApplication-EventsService) |
| **Registration Service** | Handles user event registration details | [View Repo](https://github.com/arvind20222/EventsApplication-RegistrationService) |
| **Food Option Service** | Displays available food stalls | [View Repo](https://github.com/arvind20222/EventsApplication-FoodOptionService) |
| **Payment Service** | Handles simulated payment processing | [View Repo](https://github.com/arvind20222/EventsApplication-PaymentService) |
| **Gateway Service** | Spring Cloud API Gateway for routing | [View Repo](https://github.com/arvind20222/EventsApplication-GateWay) |
| **Frontend** | React app with Bootstrap and Axios | [View Repo](https://github.com/arvind20222/EventsApplication-FrontEnd) |

---

## 🏗️ Tech Stack

| Layer | Technology |
|--------|-------------|
| Frontend | React.js, Axios, Bootstrap |
| Backend | Spring Boot, Feign Client, REST APIs |
| Database | PostgreSQL |
| Registry | Eureka Service Registry |
| Gateway | Spring Cloud Gateway |
| Tools | IntelliJ IDEA, VS Code, Postman, GitHub |
| Deployment | Render (Backend), Vercel (Frontend) |

---

## 🧠 Repository Overview

🔗 **Main Repository:**  
[Cultural Fest Management (Monorepo)](https://github.com/arvind20222/EventsApplication-Microservices-ReactJs)

```
CULTURAL_FEST_MANAGEMENT/
│
├── AdminService/
├── EventService/
├── FoodOptionService/
├── Gateway/
├── PaymentService/
├── RegistrationService/
├── UserService/
└── frontend/
```

---

## ⚙️ Setup Instructions

### 🖥️ Clone Main Repository

```bash
git clone https://github.com/arvind20222/EventsApplication-Microservices-ReactJs
cd CULTURAL_FEST_MANAGEMENT
```

### 🧩 Run Backend Services

Each service (e.g., `UserService`, `EventService`) can be run individually.

Example:
```bash
cd UserService
mvn clean install
mvn spring-boot:run
```

Ensure PostgreSQL is running and configured in:
```
src/main/resources/application.properties
```

Example:
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/userdb
spring.datasource.username=postgres
spring.datasource.password=yourpassword
```

---

### 🌉 Start API Gateway & Eureka

1. Start the **Eureka Server**
2. Start the **Gateway Service**
3. Run all microservices — they will automatically register with Eureka

---

### 💻 Frontend Setup (React)

```bash
cd frontend
npm install
npm start
```

Runs on **http://localhost:3000**

---

## 🧾 Results & Achievements

✅ 7 microservices successfully developed and integrated  
✅ Service-to-service communication via **Feign Clients**  
✅ Central routing via **Spring Cloud Gateway**  
✅ Deployed frontend (Vercel) and backend (Render)  
✅ Database: PostgreSQL with JPA and Hibernate  
✅ Clean and responsive UI with React + Bootstrap  
✅ Demonstrates **scalable microservices architecture**

---

## 🔮 Future Enhancements

- JWT-based Authentication  
- Cloud File Uploads for Event Posters  
- Email Notifications  

## 👨‍💻 Author

**Aravind Reddy**  
🔗 LinkedIn: [linkedin.com/in/aravindreddy316](https://www.linkedin.com/in/aravindreddy316)  
💻 GitHub: [github.com/aravindreddy316](https://github.com/arvind20222)

