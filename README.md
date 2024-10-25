# ⚙️ Rule Engine Application

The **Rule Engine Application** is a backend-driven rule engine built using **Java**, **Spring Boot**, **MySQL**, and **React.js**. The application evaluates custom rules based on input data and logical operators, leveraging Abstract Syntax Trees (AST) for rule processing.

---

## 🛠️ Technologies Used

- **Frontend**: React.js
- **Backend**: Java, Spring Boot 3.3.4
- **Database**: MySQL
- **Communication**: REST API (Backend exposes endpoints for rule operations)

---

## ✅ Prerequisites

- **Node.js**: Required for running the frontend.
- **Java 17+**: Ensure Java is installed by running:
  ```bash
  java -version
  ```
  
  Maven: Ensure Maven is installed by running:
  ```bash
  mvn -version
  ```
- **MySQL Database**: Set up with user credentials for database access.
- **MySQL Driver**: Make sure to include the MySQL driver in your dependencies.

## 🚀 Features
**Create Rules**: Allows users to create new rules by specifying conditions and logical operators.
**Combine Rules**: Combines multiple rules and visualizes the combined rule AST.
**Evaluate Rules**: Evaluates rules based on input data and returns results.
**REST API**: The backend provides REST endpoints to manage rules and evaluate them.
**MySQL Database**: Configured with MySQL to store rule data persistently.

## 📁 Project Structure
**Backend (Spring Boot with MySQL)**
- The Spring Boot application handles rule creation, evaluation, and combination logic. Configured with MySQL for persistent data storage, the backend runs on port 8080.

Endpoints:
- /create (POST): Creates a new rule.
- /combine (POST): Combines two or more rules.
- /evaluate (POST): Evaluates a rule with input data.


## Frontend (React.js)
- The frontend, running on port 3000, provides a user-friendly interface for creating, combining, and evaluating rules through a web UI.

## 🛠️ Setup Instructions for Rule Engine Application
**Prerequisites**
**Java 17+**: Ensure Java is installed by running:

  ```bash
  java -version
  ```
Maven: Ensure Maven is installed by running:

  ```bash
  mvn -version
  ```
**MySQL**: Set up a MySQL database and create a schema for the rule engine. Configure the backend to use this database by updating application.properties.

**Node.js**: Verify Node.js installation for running the React frontend:

  ```bash
  node -v
  npm -v
  ```

## Steps
1. **Clone the Repository**
  ```bash
  git clone https://github.com/Ankit17028/Rule-Master.git
  cd rule-engine-ast-Backend
  ```

2. **Backend Setup (In IntelliJ IDEA)**
- Configure Database in application.properties: Open src/main/resources/application.properties and set MySQL credentials:
properties

```bash
spring.datasource.url=jdbc:mysql://localhost:3306/rule_engine_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.hibernate.ddl-auto=update
```

Open Backend in IntelliJ IDEA: Open IntelliJ IDEA, select File > Open, and navigate to the rule-engine-ast/backend folder. Wait for IntelliJ to load dependencies.

Build and Run the Backend: Run the following commands in the terminal to build and run the application:

```bash
./mvnw clean install
```
After Installing mvn run the Application
```bash
./mvnw spring-boot:run
```

**Run the backend application by selecting the Application class and choosing Run. The backend server should be accessible at http://localhost:8080.**

3. **Frontend Setup (In Visual Studio Code)**
- Open Frontend in Visual Studio Code: Navigate to the frontend directory (e.g., rule-engine-ast/frontend). Open it in VS Code by running:
  
```bash
code .
```

Install Dependencies:
```bash
npm install
```
Run the Frontend Application:
```bash
npm start
```

- The frontend server should be accessible at http://localhost:3000.

# 🌐 Access the Application
Once both backend and frontend are running:

Frontend: Visit http://localhost:3000 to access the web UI.
Backend API: The backend API is available at http://localhost:8080/rules/api.

