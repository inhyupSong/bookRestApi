# RESTful book service

Simple python based RESTful service for books (in memory) in a docker container.

## Build and Run

Build: `docker build -t flaskbookapi:1.0 .`

Run: `docker run -p 5000:5000 --name FlaskBookAPI flaskbookapi:1.0`

## Use pre-built docker image

The latest image is pushed to gitlab and can be used with the following commands:

```
docker pull registry.gitlab.com/bintch/playground/restful_books:latest
docker run registry.gitlab.com/bintch/playground/restful_books:latest
```

## Access

- list: GET
- create: POST http://localhost:5000/books
- show: GET http://localhost:5000/books/1
- edit: PUT http://localhost:5000/books/1
