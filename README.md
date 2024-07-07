# API EM GOLANG

Descrição curta do projeto.

## Instalação

### Pré-requisitos

- Go 1.16 ou superior

### Clonando o Repositório

```bash
git clone https://github.com/thalisonsilva/Go-api.git

cd seu-projeto
```
### Compilando o Projeto:
```
go build -o main
```

### Executando o Projeto:
```
./main
```
### Listar Todos os Livros:
```
curl localhost:8080/books
```
### Buscar Livro por ID:
```
curl localhost:8080/books/1
```
### Criar um Novo Livro:
```
curl -X POST localhost:8080/books -H "Content-Type: application/json" -d '{"id": "4", "title": "Novo Livro", "author": "Autor Novo", "quantity": 3}'
```
### Checkout de um Livro:
```
curl -X PATCH localhost:8080/checkout?id=1
```