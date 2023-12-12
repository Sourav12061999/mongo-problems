### Queries

1.

```json
db.buyers.aggregate([{$match:{"address.state":"CA"}}])
```

--> result

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
    "_id": 4,
    "name": "Alice Lee",
    "email": "alice@example.com",
    "address": {
      "street": "321 Pine St",
      "city": "San Francisco",
      "state": "CA",
      "zip": "94101"
    }
  }
]
```
