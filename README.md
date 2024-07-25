# Spring-CRUD Example

This project is a simple Spring Boot application demonstrating basic
CRUD (Create, Read, Update, Delete) operations using an in-memory H2
database. The project is set up with Lombok to reduce boilerplate code
and uses Spring Data JPA for database interactions.


## Features - Basic CRUD operations for managing books. - Spring Boot
for application setup and configuration. - Spring Data JPA for database
interactions. - H2 in-memory database for easy setup and testing. -
Lombok for reducing boilerplate code.

## Prerequisites - Java 21 - Maven 3.8.1 or higher

## Installation 
### Clone the repository  
https://github.com/SinanUrgunWork/Spring-CRUD.git 
```
cd Spring-CRUD Build
```
### Build the project
```
mvn clean install
```
## Running the Application
```
mvn spring-boot:run
```
The application will be running at http://localhost:8080.  
## API Endpoints 
### Get all books:

`GET /api/getAllBooks`  
Response: A list of all books.  

### Get a book by ID:

`GET /api/getBookById/{id}`  
Response: A single book object.

### Add a new book:

`POST /api/addBook`  
Request body: JSON object representingthe book.  
Response: The created book object.

### Update an existing book by ID:

`POST /api/updateBook/{id}`  
Request body: JSON objectrepresenting the updated book details.  
Response: The updated book object.

### Delete a book by ID:

`DELETE /api/deleteBookById/{id}`  
Response: HTTP status OK if the book was successfully deleted.  

### Delete all books:

`DELETE /api/deleteAllBooks`  
Response: HTTP status NO CONTENT if all books were successfully deleted.

## Built With 
**Spring Boot** - Framework for building Java-based applications.  
**Spring Data JPA** - Spring Data module for JPA repositories.  
**H2 Database** - In-memory database for development and testing.  
**Lombok** - Java library to reduce boilerplate code.
