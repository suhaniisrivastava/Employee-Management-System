# Employee Management System

A Spring Boot REST API for managing employees with CRUD operations, search functionality, and MySQL integration.

## Features
- Add, update, delete, and view employees
- Search employees by name
- MySQL database integration
- Layered architecture for maintainability
- Secured endpoints with Spring Security

## Tech Stack
- Java 17
- Spring Boot
- Spring Data JPA
- Spring Security
- MySQL
- Lombok

## How to Run
1. Clone this repo:
```bash
git clone https://github.com/<your-username>/employee-management-system.git
```
2. Create MySQL DB:
```sql
CREATE DATABASE emsdb;
```
3. Update `src/main/resources/application.properties` with your DB username & password.
4. Run the application:
```bash
mvn spring-boot:run
```
5. API Endpoints:
- **GET** `/api/employees` → Get all employees
- **GET** `/api/employees/{id}` → Get employee by ID
- **POST** `/api/employees` → Add new employee
- **PUT** `/api/employees/{id}` → Update employee
- **DELETE** `/api/employees/{id}` → Delete employee
- **GET** `/api/employees/search?name=John` → Search by name

## Example Response (GET /api/employees)
```json
[
    {
        "id": 1,
        "name": "John Doe",
        "role": "Manager",
        "salary": 75000.0
    },
    {
        "id": 2,
        "name": "Jane Smith",
        "role": "Developer",
        "salary": 65000.0
    }
]
```

## Author
**Suhani Srivastava**  

---
*This project was built as part of my portfolio to showcase backend development skills using Spring Boot, MySQL, and Java.*
