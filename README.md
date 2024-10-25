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
  Maven: Ensure Maven is installed by running:
bash
Copy code
mvn -version
MySQL Database: Set up with user credentials for database access.
MySQL Driver: Make sure to include the MySQL driver in your dependencies.
🚀 Features
Create Rules: Allows users to create new rules by specifying conditions and logical operators.
Combine Rules: Combines multiple rules and visualizes the combined rule AST.
Evaluate Rules: Evaluates rules based on input data and returns results.
REST API: The backend provides REST endpoints to manage rules and evaluate them.
MySQL Database: Configured with MySQL to store rule data persistently.
📁 Project Structure
Backend (Spring Boot with MySQL)
The Spring Boot application handles rule creation, evaluation, and combination logic. Configured with MySQL for persistent data storage, the backend runs on port 8080.

Endpoints:
/create (POST): Creates a new rule.
/combine (POST): Combines two or more rules.
/evaluate (POST): Evaluates a rule with input data.
