### Query

1.

```json
db.restaurants.aggregate([
  { $match: { cuisine: "Italian" } },
  { $project: { name: 1, address: 1, _id: 0 } }
]);
```
