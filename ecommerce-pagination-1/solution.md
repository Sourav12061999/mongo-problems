<h1 style="color:#397ce7">Solution Queries:</h1>

1. db.orders.find({}).skip(3).limit(3)

- Response:

```json
[
  {
    "_id": 4,
    "customer_id": 2,
    "order_date": "2022-04-15",
    "ship_date": null,
    "status": "pending",
    "total": 100
  },
  {
    "_id": 5,
    "customer_id": 2,
    "order_date": "2022-05-01",
    "ship_date": "2022-05-05",
    "status": "shipped",
    "total": 75
  },
  {
    "_id": 6,
    "customer_id": 3,
    "order_date": "2022-05-15",
    "ship_date": "2022-05-18",
    "status": "shipped",
    "total": 50.75
  }
]
```
