<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
  db.buyers.insertMany([
  {
    "_id":6,
    "name": "Rajesh Kumar",
    "email": "rajeshkumar@example.com",
    "address": {
      "street": "123 Main St",
      "city": "New York",
      "state": "NY",
      "country": "USA",
      "zip": "10001"
    }
  },
  {
    "_id":7,
    "name": "Priya Sharma",
    "email": "priyasharma@example.com",
    "address": {
      "street": "456 Elm St",
      "city": "Los Angeles",
      "state": "CA",
      "country": "USA",
      "zip": "90001"
    }
  },
  {
    "_id":8,
    "name": "Amit Patel",
    "email": "amitpatel@example.com",
    "address": {
      "street": "789 Oak St",
      "city": "Chicago",
      "state": "IL",
      "country": "USA",
      "zip": "60601"
    }
  }
])
```
