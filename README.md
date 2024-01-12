Simple go api which returns coin balance only for a authorized user. 

Implemented with a mock database.  

```
% go run cmd/api/main.go 
Starting GO API service...
```

Use Postman or other tool to query the endpoint `http://localhost:8000/account/coins/?username=alex` with correct `Key: Authorization` and `Value: 123ABC`
This is particularly for the user `alex`. Use accordingly by looking at the mock db structure. 

It returns a JSON response with Coin Balance and status code. 

Returns error message and status code if incorrect values passed. 
