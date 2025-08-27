# BookMyShow Backend

This is a backend application inspired by BookMyShow, built with Spring Boot and MySQL.  
It provides core movie ticket booking features such as seat selection, theatre and show management, and booking flow with basic payment integration placeholder.

---

## Features

- User can book tickets  
- Seat selection during booking  
- Multiple cities supported  
- User can choose movie, theatre, show, screen, seats  
- Each theatre can have multiple screens showing different movies  
- Shows represent a movie at a specific time in a specific theatre/screen  
- View all movies in a city  
- View all shows of a chosen movie  
- Book up to 10 seats per booking  
- Seat locking to avoid double booking  
- Price depends on show and seat type  

---

## Tech Stack

- Java 17  
- Spring Boot 3.2.5  
- Maven  
- Spring Data JPA  
- Spring Web  
- Lombok  
- MySQL (Workbench for DB management)  
- IntelliJ IDEA  
- GitHub for version control  

Repository: [BookMyShow Backend](https://github.com/Ram-Git-Account/BookMyShow.git)

---

## Setup Instructions

1. Clone the repository  
   ```bash
   git clone https://github.com/Ram-Git-Account/BookMyShow.git
   cd BookMyShow
## Data Base setup for MySQL
CREATE DATABASE bookmyshow_db;
Update src/main/resources/application.properties

spring.datasource.url=jdbc:mysql://localhost:3306/bookmyshow_db
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
## Build and run the application 
mvn clean install
mvn spring-boot:run

The application will be available at http://localhost:8080
