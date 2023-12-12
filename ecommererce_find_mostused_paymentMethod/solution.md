### Queries

1.

```json
db.payments.aggregate([
  {$group:{_id:"$paymentMethod",count:{$sum:1}}},
  {$sort:{count:-1}},
  {$project:{"paymentMethod":"$_id",count:1,_id:0}},
  {$limit:1}
  ])
```

--> result

```json
[
  {
    "count": 7,
    "paymentMethod": "UPI"
  }
]
```
