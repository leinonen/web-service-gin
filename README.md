# Developing a RESTful API with Go and Gin

Download dependencies

```
go get .
```

Run the application

```
go run .
```


Get all albums

```
 curl http://localhost:8080/albums
```

Add an album

```
$ curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```

Verify that the added album is in the list

```
curl http://localhost:8080/albums
```

Get a specific album by it's ID

```
curl http://localhost:8080/albums/2
```
