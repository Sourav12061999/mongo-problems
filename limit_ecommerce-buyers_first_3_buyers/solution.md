<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.buyers.aggregate([{$limit:3}])

```

result ==>

```json
[
  {
    "_id": 2,
    "name": "Jane Doe",
    "email": "jane@example.com",
    "address": {
      "street": "456 Elm St",
      "city": "Los Angeles",
      "state": "CA",
      "zip": "90001"
    }
  },
  {
    "_id": 1,
    "name": "John Smith",
    "email": "john@hotmail.com",
    "address": {
      "street": "123 Main St",
      "city": "New York",
      "state": "NY",
      "zip": "10001"
    }
  }
]
```
