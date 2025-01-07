# Employee Management System

## Project Overview
This **Employee Management System** is a web application developed using **Spring MVC**, **Thymeleaf**, and **MySQL**. It allows administrators to manage employee data, such as adding, updating, deleting, and viewing employee information through a web interface. The system does not use JSON for data transfer, but instead interacts with the backend using traditional web forms.

## Features

### 1. **Employee CRUD Operations**
The system allows administrators to:
- **Add new employees**
- **View a list of all employees**
- **Update employee details**
- **Delete employees**

### 2. **Web Interface (Thymeleaf)**
The system has a **user-friendly web interface** built with **Thymeleaf** that provides the following views:
- **Employee List**: Displays a list of all employees in the system.
- **Employee Form**: A form to add or update employee information.
- **Employee Details**: View individual employee information.

### 3. **Database Integration**
The application uses **MySQL** as the database to store employee data. The database is connected using **JPA** and **Hibernate** for persistence management.

---

## Technologies Used
- **Spring MVC**: Framework for building the web application and handling HTTP requests.
- **Thymeleaf**: A templating engine used for rendering HTML views.
- **Spring Boot**: Used to set up and run the application.
- **Spring Data JPA**: For database interaction with **MySQL**.
- **MySQL**: Relational database to store employee data.

---

## Getting Started

### Prerequisites
Make sure you have the following installed:
- **JDK 17+**
- **Maven** (or any build tool you prefer)
- **MySQL Database**

### Setting up the Database
1. Create a **MySQL** database named `employee_management`.
2. Update the `application.properties` file with your database credentials:
    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/employee_management
    spring.datasource.username=root
    spring.datasource.password=your_password
    spring.jpa.hibernate.ddl-auto=update
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    ```

### Running the Application
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/EmployeeManagementSystem.git
    ```
2. Navigate to the project directory:
    ```bash
    cd EmployeeManagementSystem
    ```
3. Build and run the application using **Maven**:
    ```bash
    mvn spring-boot:run
    ```

4. Access the application in your browser:
    - **Web Interface**: [http://localhost:8080/employees/list](http://localhost:8080/employees/list)

---

## Contributing
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -am 'Add feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Create a pull request.

---

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
