# To run service
```
go run .
```

# APIs
## To get all albums
```
curl http://localhost:8080/albums
```

## To get album by id

```
curl http://localhost:8080/albums/1
```


## To add new album
```
curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```

## To remove album by id
```
curl -X DELETE http://localhost:8080/albums/1
```
