# <h1 align = "center"> 🎓Ecommerce App🎓 </h1>
___ 
<p align="center">
<a href="Java url">
    <img alt="Java" src="https://img.shields.io/badge/Java->=8-darkblue.svg" />
</a>
<a href="Maven url" >
    <img alt="Maven" src="https://img.shields.io/badge/maven-3.1.3-brightgreen.svg" />
</a>
<a href="Spring Boot url" >
    <img alt="Spring Boot" src="https://img.shields.io/badge/Spring Boot-3.0.6-brightgreen.svg" />
</a>
</p>

---

<p align="left">

<!-- Project Description -->
## Overview 🪟
<p align="center">This project, named "Ecommerce App," is a robust Spring Boot application designed for managing user data efficiently. It provides a set of API endpoints that allows you to manage User,Product, Address and Order to perform CRUD operations, and apply the specified validations. The application will use MySQL as the database for simplicity and we have use validation as well.
</p>

<!-- Table of Contents -->
## Table of Contents📑
1. [Technologies Used](#technologies-used)
2. [Models Key Feautures](#models-key-features🔑)
3. [Usage](#usage)
4. [Controller](#controller🎮)
5. [Endpoint API reference](#endpoint-api-reference)
6. [Acknowledgments](#acknowledgments)
7. [Contact](#contact)

<!-- Technologies Used -->
## Technologies Used🧑‍💻
- Java 21
- Spring Boot
- Spring Web Initializer
- Maven 
- Spring Web Dependency  { Spring web, Lombok, Validation, MySQL Databse, Spring JPA, Swagger, Hibernate}
- MySQL


<!-- Model --->

## Models Key Features🔑
### 1 -> User Model
    Attribute's
       -> d:integer
       -> name:string
       -> email:string
       -> password:string
       -> phoneNumber:string
 

### 2 -> Address Model
    Attributes's
       ->  id:integer    
       -> name:string
       -> landmark:string
       -> phoneNumber:string
       -> zipcode:string
       -> state:string
       -> UserID : foreign key mapping

 ### 1 -> Product Model
    Attribute's
       -> id:integer 
       -> name:string
       -> price:integer
       -> description:string
       -> category:string
       -> brand:string

### 2 -> Order Model
    Attributes's
      -> id:integer
      -> userID:integer (foreign key mapping)
      -> productID:integer(foreign key mapping)
      -> addressID:integer(foreign key mapping)
      -> productQuantity:integer

<!-- Usage -->
## Usage
- Access the application at `http://localhost:8081`.
- Use the provided API endpoints to manage your User Management.

### Controller🎮:
- It consists of a class named APIController which basically controls the flow of data.
- @RestController annotation is used to make the APIController as a controller layer.
- We perform the CRUD operations such as @PostMapping , @GetMapping , @PutMapping , @DeleteMapping.

### Endpoint API Reference :

         -> Add users
         -> Add products
         -> Add Address
         -> Place an order (Create Order) using userId,     productId, addressId
         -> Get order by order id
         -> Get user by userid
         -> Get all products
         -> Get products based on category (query params) 
         -> delete products based on product id.
 

 <!-- Acknowledgments -->
## Acknowledgments
- Thank you to the Spring Boot and Java communities for providing excellent tools and resources.

<!-- Contact -->
## Contact📲
For questions or feedback, please contact : Avadhesh Shukla👍
- Maild Id 📧: avadheshsukla1636@gmail.com

<h1 align="center">Thank You💖...<h1>
<h3 align = "center"> ***********************************************************<h3>




 
