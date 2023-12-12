### Query

1.

```json
db.restaurants.aggregate([ { $group: { _id: "$cuisine", count: { $sum: 1 } } }, { $sort: { count: -1 } }, { $limit: 5 }]);
```
