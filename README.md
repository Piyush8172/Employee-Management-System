# Java Full Stack – Employee Management System

A full-stack **Employee Management System** built using **React.js, Spring Boot, and MySQL**. The application provides CRUD operations for managing employee records and demonstrates REST API integration between the React frontend and Spring Boot backend.

## 🚀 Tech Stack

### Frontend

* React.js
* HTML5
* CSS3
* JavaScript
* Axios

### Backend

* Java
* Spring Boot
* Spring Data JPA
* Hibernate
* REST APIs

### Database

* MySQL

### Tools

* Git & GitHub
* Postman
* IntelliJ IDEA / Eclipse
* VS Code

## ✨ Features

* Add new employees
* View all employees
* View employee details
* Update employee information
* Delete employees
* RESTful API integration
* MySQL database integration
* React-based responsive user interface
* Backend validation and exception handling
* Layered Spring Boot architecture

## 🏗️ Project Architecture

```text
                    Employee Management System
                              │
                 ┌────────────┴────────────┐
                 │                         │
           React Frontend            Spring Boot Backend
                 │                         │
              Axios                    REST APIs
                 │                         │
                 └────────────┬────────────┘
                              │
                         Spring Data JPA
                              │
                           Hibernate
                              │
                           MySQL DB
```

## 📂 Project Structure

```text
Java-Full-Stack-Project-Code/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── services/
│   │   ├── App.js
│   │   └── index.js
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── ...
│   │   │   └── resources/
│   │   │       └── application.properties
│   │   └── test/
│   ├── pom.xml
│   └── ...
│
└── README.md
```

> The exact folder structure may vary depending on the project configuration.

## 🔗 REST API Endpoints

| Method   | Endpoint              | Description           |
| -------- | --------------------- | --------------------- |
| `GET`    | `/api/employees`      | Get all employees     |
| `GET`    | `/api/employees/{id}` | Get employee by ID    |
| `POST`   | `/api/employees`      | Create a new employee |
| `PUT`    | `/api/employees/{id}` | Update an employee    |
| `DELETE` | `/api/employees/{id}` | Delete an employee    |

## 🗄️ Database Configuration

Create a MySQL database:

```sql
CREATE DATABASE employee_management;
```

Configure the database connection in:

```text
src/main/resources/application.properties
```

Example:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/employee_management
spring.datasource.username=root
spring.datasource.password=YOUR_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
```

Replace `YOUR_PASSWORD` with your MySQL password.

## ⚙️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/Piyush8172/Employee-Management-System.git
```

```bash
cd Employee-Management-System
```

### 2. Start MySQL

Make sure MySQL Server is running and create the required database.

### 3. Run the Spring Boot Backend

Open the backend project in IntelliJ IDEA or Eclipse and run the Spring Boot application.

The backend will typically run on:

```text
http://localhost:8080
```

### 4. Run the React Frontend

Navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the React application:

```bash
npm start
```

The frontend will typically be available at:

```text
http://localhost:3000
```

## 🔄 Application Flow

```text
User
  │
  ▼
React UI
  │
  ▼
Axios HTTP Request
  │
  ▼
Spring Boot REST Controller
  │
  ▼
Service Layer
  │
  ▼
Repository Layer
  │
  ▼
MySQL Database
  │
  ▼
Response
  │
  ▼
React UI
```

## 🧩 Backend Layered Architecture

The backend follows a layered architecture:

```text
Controller
    ↓
Service
    ↓
Repository
    ↓
Database
```

### Controller

Handles incoming HTTP requests and exposes REST API endpoints.

### Service

Contains the application's business logic.

### Repository

Uses Spring Data JPA to communicate with the MySQL database.

### Entity

Represents employee data as Java objects and maps them to database tables using JPA/Hibernate.

## 📌 Key Learning Outcomes

Through this project, I gained practical experience in:

* Java and Spring Boot development
* Building RESTful APIs
* CRUD operations
* Spring Data JPA and Hibernate
* MySQL database integration
* React.js frontend development
* Frontend-backend API integration
* Layered application architecture
* API testing using Postman
* Git and GitHub version control

## 🔮 Future Enhancements

* Add user authentication and authorization using Spring Security/JWT
* Add employee search and filtering
* Add pagination and sorting
* Improve form validation
* Add role-based access control
* Deploy the application on a cloud platform

## 👨‍💻 Author

**Piyush Gupta**

Java | Spring Boot | React.js | MySQL | REST APIs | Cloud

---

⭐ If you find this project useful, consider giving the repository a star!
