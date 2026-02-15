# DevOps Lab 03: Product Service Microservice 

This project is a **Spring Boot RESTful microservice** developed for **SE4010 – Current Trends in Software Engineering**. It serves as a hands-on implementation of microservice architecture, focusing on CRUD operations, persistence, and API documentation.

---

## 🛠 Technologies Used

| Category | Technology |
| :--- | :--- |
| **Language** | Java 21 |
| **Framework** | Spring Boot 3.x |
| **Database** | H2 (In-Memory) |
| **API Docs** | Swagger / OpenAPI (Springdoc) |
| **Build Tool** | Maven |
| **Version Control** | Git & GitHub |

---

## ✨ Features

* **Full CRUD Lifecycle:** Create, Read (All/ID), and Delete products.
* **Persistent In-Memory Storage:** Uses H2 database for rapid development and testing.
* **Interactive API Documentation:** Integrated Swagger UI for testing endpoints without external tools.
* **Layered Architecture:** Clean separation of concerns between Controllers, Models, and Repositories.

---

## 📂 Project Structure

src/main/java/com/example/productservice/
├── controller/    # REST API Endpoints
├── model/         # JPA Entity classes (Product)
├── repository/    # Data Access Layer (Spring Data JPA)
└── ProductserviceApplication.java # Application Entry Point


## ⚙️ Setup & Installation
## Prerequisites
* **JDK 21 or higher**

* **Maven 3.6+**

* **IDE (IntelliJ, VS Code, or Eclipse)**

## Run the Application
* **1.Clone the repository:**
* Bash
* git clone <your-repo-url>
*cd productservice

* **2.Build and Run using Maven:**
* Bash
* mvn spring-boot:run
  
## 🌐 API Access & Documentation

Once the application is running, you can access the following interfaces:

Swagger UI : http://localhost:8081/swagger-ui/index.html
H2 Console : http://localhost:8081/h2-console

## 🗄️ Database Credentials (H2)
JDBC URL: jdbc:h2:mem:testdb

Username: sa

Password: (leave blank)

## 🧪 Example Usage
Create a Product
POST /api/products

JSON
{
  "name": "Gaming Laptop",
  "price": 1200.50
}
Get All Products
GET /api/products
