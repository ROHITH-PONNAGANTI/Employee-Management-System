# Employee-Management-System
A decoupled, modern full-stack enterprise user management application. This project features a responsive React single-page application (SPA) frontend that communicates via a RESTful API with a robust Java Spring Boot backend, utilizing a persistent MySQL database layer.

## 🚀 Live Links & Architecture
* **Frontend Client:** React / Axios / Bootstrap
* **Backend API:** Java / Spring Boot / Spring Data JPA
* **Database Layer:** MySQL Core Engine

---

## 👨‍💻 Description
* **Architected a decoupled, full-stack Employee Management system** using **React** and **Spring Boot**, separating concerns to ensure independent deployment scalability and optimal client-side rendering.
* **Engineered a comprehensive RESTful API** supporting full CRUD operations by leveraging **Spring Data JPA/Hibernate**, enabling automated database schema generation and reducing boilerplate SQL by **100%**.
* **Optimized application resilience** by implementing a centralized, custom global exception handling layer (`UserNotFoundException`), resulting in clean **HTTP 404/500 error mapping** and preventing backend crash leakage to the UI.
* **Implemented dynamic state management and routing** using **React Router DOM**, achieving seamless **single-page application (SPA)** transitions without full-page reloads, significantly lowering network overhead.
* **Secured cross-origin data exchanges** by configuring a custom **CORS (Cross-Origin Resource Sharing)** policy wrapper on the backend, safely unlocking seamless communication between independent local and cloud host ports.

---

## 🛠️ Tech Stack & Dependencies

### Frontend
* **Core Framework:** React.js (v18+)
* **Styling & Layout:** Bootstrap 5 (Responsive Layout Grids)
* **HTTP Client:** Axios (Promise-based asynchronous requests)
* **Routing:** React Router DOM (Declarative client-side routing)

### Backend & Database
* **Language:** Java 17
* **Framework:** Spring Boot (v2.6.7)
* **ORM / Data Access:** Hibernate / Spring Data JPA
* **Database:** MySQL 8.0
* **Build Tool:** Maven (Wrapper included)

---

## ⚙️ Local Development Setup

### 1. Database Configuration
Before booting up the backend application, ensure MySQL is running locally and initialize the database schema:
```sql
CREATE DATABASE fullstack;
Verify your connection parameters inside the backend folder under src/main/resources/application.properties:

Properties
spring.datasource.url=jdbc:mysql://localhost:3006/fullstack
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD
spring.jpa.hibernate.ddl-auto=update
2. Backend Execution (Spring Boot)
Navigate to the root directory of the backend folder and launch the embedded Apache Tomcat container:

Bash
# Windows PowerShell
.\mvnw spring-boot:run

# Windows Command Prompt or macOS/Linux Terminal
./mvnw spring-boot:run
The console will verify a successful boot sequence with:

Tomcat started on port(s): 8080 (http) with context path ''

3. Frontend Execution (React Client)
Navigate to the root directory of the frontend folder, install dependencies, and start the local Webpack development server:

Bash
# Install node modules
npm install

# Run application client
npm start
The application will automatically launch and open your default web browser to: http://localhost:3000
