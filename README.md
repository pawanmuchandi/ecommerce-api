 Simple E-commerce API – Java + Spring Boot
A simple e-commerce REST API built using Java, Spring Boot, JWT Authentication, and MySQL. This project is designed to simulate the core backend features of an online shopping platform including user login, product listing, cart management, and order creation.

🚀 Features
✅ User Authentication with JWT

👤 Two User Roles:

CUSTOMER: Can view products, manage cart, and place orders.

ADMIN: Can manage (add/update/delete) products.

📦 Product Listings

🛒 Cart Management

🧾 Order Creation

🔐 JWT-based Role Access Control

🌐 RESTful API using Spring Boot

🛠️ Technologies Used
Java 21

Spring Boot 3.5.3

Spring Security

Spring Data JPA

MySQL

JWT (Java Web Tokens)

Lombok

Maven

📂 API Endpoints Overview
🔑 Authentication
Method	Endpoint	Description
POST	/auth/register	Register a user
POST	/auth/login	Login and get token

📦 Products
Method	Endpoint	Access	Description
GET	/products	All users	View all products
POST	/products	Admin only	Add a new product
PUT	/products/{id}	Admin only	Update product details
DELETE	/products/{id}	Admin only	Delete a product

🛒 Cart & Orders (in development or optional extension)
🧪 How to Run
Clone the repo:

bash
Copy
Edit
git clone https://github.com/your-username/ecommerce-api.git
cd ecommerce-api
Configure your application.properties:

properties
Copy
Edit
spring.datasource.url=jdbc:mysql://localhost:3306/ecommerce
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
Run the app:

bash
Copy
Edit
mvn spring-boot:run
Test using Postman or a basic frontend HTML page.

✍️ Author
Pawan Muchandi
Java Full Stack Developer# ecommerce-api
