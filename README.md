# Online Bookstore Management System

This project is an **Online Bookstore Management System** built using **Spring Boot** and **Spring Data JPA**. It provides a REST API for managing books in the bookstore, allowing you to perform CRUD (Create, Read, Update, Delete) operations and view the total number of books in the database.

## Features

- Add a new book to the store
- Retrieve a book by its ID
- Retrieve all books in the store
- Delete a specific book by its ID
- Delete all books
- Get the total count of books

## Technologies Used

- Java
- Spring Boot
- Spring Data JPA
- Hibernate
- MySQL (or any relational database)
- REST API

## Project Structure


## API Endpoints

The following endpoints are exposed by the `BookController`:

| Method   | Endpoint           | Description                      |
|----------|--------------------|----------------------------------|
| `POST`   | `/books/add`        | Add a new book                   |
| `GET`    | `/books/{id}`       | Get a book by its ID             |
| `GET`    | `/books/all`        | Get all books                    |
| `DELETE` | `/books/{id}`       | Delete a book by its ID          |
| `DELETE` | `/books/all`        | Delete all books                 |
| `GET`    | `/books/count`      | Get the total number of books    |

## How to Run

1. Clone the project repository:

```bash
git clone https://github.com/your-username/bookstore-management-system.git
cd bookstore-management-system
spring.datasource.url=jdbc:mysql://localhost:3306/bookstoredb
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
mvn spring-boot:run

POST /books/add
Content-Type: application/json

{
  "bookId": 1,
  "title": "Spring Boot in Action",
  "author": "Craig Walls",
  "price": 35.99
}


This `README.md` file provides a clear overview of the project, its structure, technologies used, API endpoints, and steps to run the application. Adjust the details based on your actual project setup.

