### Queries

1.

```json
db.buyers.aggregate([
    {$match:{_id:1}},
    {$lookup:{from:"orders",localField:"_id",foreignField:"customer_id",as:'orders'}},
    {$project:{orders:1}}
    ]);
```

    --> result for buyers id 1

```json
[
  {
    "_id": 1,
    "orders": [
      {
        "_id": 1,
        "customer_id": 1,
        "order_date": "2022-03-01",
        "ship_date": "2022-03-05",
        "status": "shipped",
        "total": 50.25
      },
      {
        "_id": 2,
        "customer_id": 1,
        "order_date": "2022-03-15",
        "ship_date": "2022-03-18",
        "status": "shipped",
        "total": 25.5
      },
      {
        "_id": 3,
        "customer_id": 1,
        "order_date": "2022-04-01",
        "ship_date": null,
        "status": "pending",
        "total": 75
      }
    ]
  }
]
```
