### Queries

1.  db.orders.aggregate([{$group: {_id: null, total: {$sum: "$total"}}},{$project:{_id:0}}])

- Expected output

```json
[{ "total": 687.75 }]
```
