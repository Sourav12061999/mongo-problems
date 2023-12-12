### Query

1.

```json
db.restaurants.aggregate([
  { $match: { cuisine: { $in: ["Italian", "Mexican"] } } }
]);
```
