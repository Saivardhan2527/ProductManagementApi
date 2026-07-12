# 🛍️ Product Management API

A RESTful Product Management API built using **Spring Boot**, **MongoDB**, and **Maven**. This project demonstrates CRUD (Create, Read, Update, Delete) operations on products using REST APIs.

---

## 📌 Features

- ➕ Add a new product
- 📋 View all products
- 🔍 View a product by ID
- ✏️ Update product details
- ❌ Delete a product
- 🍃 MongoDB integration
- 🌐 RESTful API architecture
- 🧪 API testing using Postman

---

## 🛠️ Technologies Used

- Java 23
- Spring Boot 3.4.1
- Spring Data MongoDB
- MongoDB
- Maven
- REST API
- Postman

---

## 📂 Project Structure

```
ProductManagementApi
│
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com.example
│   │   │       ├── controller
│   │   │       ├── model
│   │   │       ├── repository
│   │   │       ├── service
│   │   │       └── Main.java
│   │   │
│   │   └── resources
│   │       ├── static
│   │       └── application.properties
│   │
│   └── test
│
├── .mvn
├── mvnw
├── mvnw.cmd
├── pom.xml
└── README.md
```

---

## ⚙️ Prerequisites

Before running the project, ensure you have:

- Java JDK 17 or later (Java 23 recommended)
- Apache Maven 3.9+
- MongoDB
- Git
- Postman (for API testing)

---

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Saivardhan2527/ProductManagementApi.git
```

### 2. Navigate to the Project

```bash
cd ProductManagementApi
```

### 3. Configure MongoDB

Update the `application.properties` file with your MongoDB configuration.

Example:

```properties
spring.data.mongodb.host=YOUR_HOST
spring.data.mongodb.port=YOUR_PORT
spring.data.mongodb.database=YOUR_DATABASE
spring.data.mongodb.username=YOUR_USERNAME
spring.data.mongodb.password=YOUR_PASSWORD
```

### 4. Build the Project

```bash
mvn clean install
```

### 5. Run the Application

```bash
mvn spring-boot:run
```

The application will start at:

```
http://localhost:8080
```

---

# 📡 API Endpoints

## Create Product

**POST**

```
http://localhost:8080/api/products
```

### Request Body

```json
{
    "name":"Laptop",
    "description":"Gaming Laptop",
    "price":65000,
    "quantity":20,
    "category":"Electronics"
}
```

---

## Get All Products

**GET**

```
http://localhost:8080/api/products
```

---

## Get Product by ID

**GET**

```
http://localhost:8080/api/products/{id}
```

---

## Update Product

**PUT**

```
http://localhost:8080/api/products/{id}
```

### Request Body

```json
{
    "name":"Laptop",
    "description":"Updated Gaming Laptop",
    "price":70000,
    "quantity":15,
    "category":"Electronics"
}
```

---

## Delete Product

**DELETE**

```
http://localhost:8080/api/products/{id}
```

---

# 🧩 Project Architecture

```
Client (Postman / Browser)
           │
           ▼
   ProductController
           │
           ▼
    ProductService
           │
           ▼
 ProductRepository
           │
           ▼
        MongoDB
```

---

# 📷 Testing

Use **Postman** to test all CRUD APIs.

- POST → Create Product
- GET → View Products
- PUT → Update Product
- DELETE → Remove Product

---

# 📚 Learning Outcomes

This project helped me understand:

- Spring Boot Project Structure
- REST API Development
- CRUD Operations
- Spring Data MongoDB
- Maven Build Tool
- Dependency Injection
- MVC Architecture
- API Testing with Postman

---

# 👨‍💻 Author

**Saivardhan Kolakani**

- GitHub: https://github.com/Saivardhan2527

---

## ⭐ If you found this project useful, consider giving it a star!
