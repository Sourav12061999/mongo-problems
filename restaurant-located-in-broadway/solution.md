### Query

1.

```json
db.restaurants.aggregate([
  {
    $match: { "address.street": "Broadway" }
  },
  {
    $sort: { "address.zipcode": 1 }
  },
  {
    $limit: 10
  }
])
```
