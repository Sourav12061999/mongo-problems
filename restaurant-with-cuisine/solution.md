### Query

1.

```json
db.restaurants.aggregate([
  { $project: { name: 1, cuisine: 1, _id: 0 } }
])
```
