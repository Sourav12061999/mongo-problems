<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([{$sort:{total:-1}}])

```

result ==>

```json
[
  {
    "_id": 9,
    "customer_id": 4,
    "order_date": "2022-07-01",
    "ship_date": "2022-07-05",
    "status": "shipped",
    "total": 125.5
  },
  {
    "_id": 4,
    "customer_id": 2,
    "order_date": "2022-04-15",
    "ship_date": null,
    "status": "pending",
    "total": 100
  }
]
```
