### Queries

1.

```json
db.orders.aggregate([
  { $group: { _id: "$status", count: { $sum: 1 } } }
])
```
