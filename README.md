# API EM GOLANG

Este projeto consiste em uma API em Go para gerenciar um catálogo de livros. Utiliza o framework Gin para facilitar a criação de endpoints HTTP.

## Funcionalidades Principais

- Listagem de todos os livros disponíveis.
- Busca de um livro por ID.
- Adição de novos livros ao catálogo.
- Funcionalidade de checkout para emprestar livros.

## Tecnologias Utilizadas

- Go 1.16
- Gin (github.com/gin-gonic/gin) - Framework web para Go
- JSON - Formato utilizado para comunicação entre cliente e servidor

## Instruções de Uso

### Clonando o Repositório

```bash
git clone https://github.com/thalisonsilva/Go-api.git
cd seu-projeto


cd seu-projeto
```
### Compilando o Projeto:
```
go build -o main

### Executando o Projeto:
```
./main

### Listar Todos os Livros:

```
curl localhost:8080/books

### Buscar Livro por ID:

curl localhost:8080/books/1

### Criar um Novo Livro:

```
curl -X POST localhost:8080/books -H "Content-Type: application/json" -d '{"id": "4", "title": "Novo Livro", "author": "Autor Novo", "quantity": 3}'

### Checkout de um Livro:
```
curl -X PATCH localhost:8080/checkout?id=1