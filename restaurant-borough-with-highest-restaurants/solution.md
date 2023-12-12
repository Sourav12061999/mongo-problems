### Query

1.

```json
db.restaurants.aggregate([
  { $group: { _id: "$borough", count: { $sum: 1 } } },
  { $sort: { count: -1 } },
  { $limit: 1 }
])
```
