# **Employee Management System**

This is a Spring Boot-based Employee Management System that enables users to perform CRUD (Create, Read, Update, Delete) operations on employee records. It serves as an example of building a modern REST API using Java and Spring.

---

## **Features**
- Add, update, view, and delete employee records.
- Database integration using JPA and Hibernate.
- RESTful APIs for backend services.
- Minimal setup for running the application.

---

## **Technologies Used**
- **Backend**: Java, Spring Boot
- **Frontend**: Typescript, Angular
- **Database**: MySQL/PostgreSQL(or replaceable with H2 )
- **Build Tool**: Maven
- **IDE Support**: IntelliJ IDEA.

---

## **Setup and Installation**

### Prerequisites
- Java 17 or higher.
- Maven 3.8 or higher.
- IDE for Java development (e.g., IntelliJ IDEA).
- Postgres database (pre-configured) or your preferred database.

### Clone the Repository
```bash
git clone https://github.com/WangariNelly/Employee-Management-System
cd employeemanagementsystem
```

### Configure Database
- Open `src/main/resources/application.properties`.
- Configure your database settings if needed. Default configuration uses H2:
  ```properties
  spring.datasource.url=jdbc:postgresql://localhost:5432/employeemanager
  spring.datasource.username=
  spring.datasource.password=
  spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
  spring.jpa.hibernate.ddl-auto=update
  spring.jpa.show-sql=true
  ```

### Build and Run the Application
- **Using Maven**:
  ```bash
  mvn spring-boot:run
  ```
- **Using IDE**:
    1. Open the project in your IDE.
    2. Run the `EmployeeManagerApplication` class.

### Access the Application
- REST API Documentation: `http://localhost:8080/swagger-ui/` (if Swagger is enabled).
- Default API Endpoint: `http://localhost:8080/api/employees`.

---

## **API Endpoints**

### Employee Management
- **GET /api/employees**: Fetch all employees.
- **POST /api/employees**: Add a new employee.
- **PUT /api/employees/{id}**: Update an employee by ID.
- **DELETE /api/employees/{id}**: Delete an employee by ID.

---

## **Contributing**
Feel free to fork this repository and submit pull requests to improve the project.

---

