### Queries

1. db.transactions.aggregate([ { $unwind: "$transactions" }, { $group: { _id: "$account_id", count: { $sum: 1 } } }])

- Expected Output -

```
[
  { _id: 557378, count: 10 },
  { _id: 198100, count: 4 },
  { _id: 278603, count: 14 },
  { _id: 674364, count: 14 }
]
```
