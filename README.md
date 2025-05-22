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


## API ENDPOINTs
1. **Get All Movies**
```bash
GET /movies
```
Returns a list of all movies. <br/>
2. **Get a Movie by ID**
```bash
GET /movies/{id}
```
Returns the movie with the specified ID. <br/>
3. **Create a New Movie**
```bash
POST /movies
```
```JSON

{
  "isbn": "12345",
  "title": "New Movie",
  "director": {
    "firstname": "John",
    "lastname": "Doe"
  }
}
```

4. **Update a Movie**
```bash
PUT /movies/{id}
```
```JSON

{
  "isbn": "67890",
  "title": "Updated Movie",
  "director": {
    "firstname": "Jane",
    "lastname": "Smith"
  }
}
```
5. **Delete a Movie**
```bash
DELETE /movies/{id}
```
Deletes the movie with the specified ID.