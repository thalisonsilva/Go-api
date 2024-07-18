# API IN GOLANG

This project consists of a Go API to manage a book catalog. Uses the Gin framework to facilitate the creation of HTTP endpoints.

## Main Features

- List of all available books.
- Search for a book by ID.
- Addition of new books to the catalogue.
- Checkout functionality to borrow books.

## Technologies Used

- Go 1.16
- Gin (github.com/gin-gonic/gin) - Web framework for Go
- JSON - Format used for communication between client and server

## Instructions for use

### Cloning the Repository


`git clone https://github.com/thalisonsilva/Go-api.git
cd your-project`

### Compiling and Running the Project

`go build -o main
./main`

### Usage Examples
List All Books:

`curl localhost:8080/books`

### Search Book by ID:

`curl localhost:8080/books/1`

### Create a New Book:


`curl -X POST localhost:8080/books -H "Content-Type: application/json" -d '{"id": "4", "title": "New Book", "author": "New Author" , "quantity": 3}'`

### Checkout a Book:

`curl -X PATCH localhost:8080/checkout?id=1`
