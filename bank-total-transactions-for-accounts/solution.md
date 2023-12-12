### Queries

1. db.transactions.aggregate([ { $unwind: "$transactions" }, { $group: { _id: "$account_id", total_amount: { $sum: "$transactions.amount" } } }])

- Expected Output -

```
[
  { _id: 557378, total_amount: 39607 },
  { _id: 198100, total_amount: 21169 },
  { _id: 278603, total_amount: 69629 },
  { _id: 674364, total_amount: 78962 }
]
```
