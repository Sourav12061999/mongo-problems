### Query

1.

```json
db.restaurants.aggregate([ { $unwind: "$grades" }, { $sort: { "grades.date": -1 } }, { $limit: 1 }, { $project: { name: 1, "grades.date": 1, _id: 0 } }])
```

- Expected Output -

```
[
  {
    grades: { date: '2015-01-09T00:00:00.000Z' },
    name: 'Bagels N Buns'
  }
]
```
