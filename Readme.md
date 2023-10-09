# <h1 align = "center"> 🎓Student_Portal_With_Mappings🎓 </h1>
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
<p align="center">This project, named "Student_Portal_With_Mappings" is a robust Spring Boot application designed for managing user data efficiently. It provides a set of API endpoints with mappings that allows you to manage Student, Laptop, Course, Book and Address to perform CRUD operations, and apply the specified validations. The application will use MySQL as the database for simplicity and we have use validation as well.
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
### 1 -> Student Model
    Attribute's
       ->private String ID;
       -> private String name;
       -> private String age;
       -> private String phoneNumber;
       -> private String branch;
       -> private String department;

         @OneToOne
       -> private Address address;

         @OneToMany
       -> Set<course> courseSet;
 

### 2 -> Course Model
    Attributes's
       -> private String ID;
       -> private String title;
       -> private String description;
       -> private String duration;

         @ManyToMany
       -> Set<Student> studentSet;

 ### 1 -> Laptop Model
    Attribute's
       ->  private String ID;
       -> private String name;
       -> private String brand;
       -> private Integer price;
         @OneToOne
       -> private Student student;

### 2 -> Book Model
    Attributes's
      -> private String ID;
      -> private String title;
      -> private String author;
      -> private String description;
      -> private String price;

         @ManyToOne
      -> private Student student;

### 2 -> Address Model
    Attributes's
      -> private Long addressId;
      -> private String landmark;
      -> private String zipcode;
      -> private String district;
      -> private String state;
      ->private String country;


<!-- Usage -->
## Usage
- Access the application at `http://localhost:8080`.
- Use the provided API endpoints to manage your User Management.

### Controller🎮:
- It consists of a class named APIController which basically controls the flow of data.
- It consists mapping like OneToOne , ManyToOne, OneToMany and ManyTomany.
- @RestController annotation is used to make the APIController as a controller layer.
- We perform the CRUD operations such as @PostMapping , @GetMapping , @PutMapping , @DeleteMapping.

### Endpoint API Reference :

    Performed CRUD operation in every Model :- 
      - Post
      - Get
      - Put
      - Delete
    

 <!-- Acknowledgments -->
## Acknowledgments
- Thank you to the Spring Boot and Java communities for providing excellent tools and resources.

<!-- Contact -->
## Contact📲
For questions or feedback, please contact : Avadhesh Shukla👍
- Maild Id 📧: avadheshsukla1636@gmail.com

<h1 align="center">Thank You💖...<h1>
<h3 align = "center"> ***********************************************************<h3>




 
