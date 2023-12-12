<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.buyers.aggregate([{$skip:1},{$limit:2}])

```

result ==>

```json
[ {
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
    "_id": 3,
    "name": "Bob Johnson",
    "email": "bob@example.com",
    "address": {
      "street": "789 Oak St",
      "city": "Chicago",
      "state": "IL",
      "zip": "60601"
    }
  }
]
```
