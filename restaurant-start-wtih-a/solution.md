### Query

1.

```json
db.restaurants.aggregate([
  {
    $match: { cuisine: /^A/ }
  },
  {
    $sort: { name: 1 }
  },
  {
    $limit: 10
  }
])
```
