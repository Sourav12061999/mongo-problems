### Query

1.

```json
db.restaurants.aggregate([ { $match: { cuisine: "Turkish" } }, { $unwind: "$grades" }, { $group: { _id: "$name", avgScore: { $avg: "$grades.score" } } }, { $sort: { avgScore: -1 } }])
```

- Expected Output -

```json
[{ "_id": "The Country Cafe", "avgScore": 10.5 }]
```
