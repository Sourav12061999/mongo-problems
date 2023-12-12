### Queries

1. db.orders.aggregate([ { $group: { _id: "$customer_id", count: { $sum: 1 } } }])

- Expected output

```json
[
  { "_id": 1, "count": 3 },
  { "_id": 5, "count": 2 },
  { "_id": 2, "count": 2 },
  { "_id": 3, "count": 3 },
  { "_id": 4, "count": 1 }
]
```
