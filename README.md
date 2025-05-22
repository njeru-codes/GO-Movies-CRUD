# 🎬 Go Movie REST API
This is a simple RESTful API built with Go and the Gorilla Mux router. It allows users to perform CRUD operations on a list of movies.

## FEATURES
- `GET`     `/movies`  Get all movies
- `GET` `/movies/id` Get specific movie by id
- `POST` `/movies` create a new movie record
- `PUT` `/movies/id`  update exisitng movie
- `DELETE` `/movies/id`   delete a movie

## Getting started
1. install dependencies
```
go get -u github.com/gorilla/mux
```
2. run the server
```
go run main.go
```
server will start on `http://localhost:8000`