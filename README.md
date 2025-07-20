# 🎓 StudentPortalAPI

### 📌 **Description**
StudentPortalAPI is a **Spring Boot based RESTful API** for managing student registrations with **secure JWT authentication** and role-based access. It allows registration, authentication, CRUD operations, and role management of students in an educational system.

---

### 🚀 **Features**
✅ Register new students with encoded passwords  
✅ JWT token-based authentication  
✅ Role-based authorization (ADMIN role to manage students)  
✅ Get all students, get by ID  
✅ Full update and partial update of student information  
✅ Delete student record  
✅ PostgreSQL integration  
✅ Custom user details service for authentication  
✅ Bean validation for data integrity

---

### 💻 **Tech Stack**
- Java 17
- Spring Boot 3.5.3
- Spring Security
- Spring Data JPA
- JWT (io.jsonwebtoken)
- PostgreSQL
- Maven/Gradle
- Hibernate Validator

---

📡 API Endpoints

| Method | Endpoint            | Description                    | Authorization |
| ------ | ------------------- | ------------------------------ | ------------- |
| POST   | `/api/register`     | Register new student           | Public        |
| POST   | `/api/authenticate` | Authenticate and get JWT token | Public        |
| GET    | `/api/students`     | Get all students               | ADMIN         |
| GET    | `/api/student/{id}` | Get student by ID              | ADMIN         |
| PUT    | `/api/student/{id}` | Full update student            | ADMIN         |
| PATCH  | `/api/student/{id}` | Partial update student         | ADMIN         |
| DELETE | `/api/student/{id}` | Delete student                 | ADMIN         |


🔑 Authentication
Register a new student via /api/register.
Login via /api/authenticate with JSON body:
{
  "login": "studentLogin",
  "password": "studentPassword"
}

👨‍💻 Author
Muhammadali Qoxxoraliyev
Backend Developer | Spring Boot | Java
