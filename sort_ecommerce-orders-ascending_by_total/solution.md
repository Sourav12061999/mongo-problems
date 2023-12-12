<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([{$sort:{total:1}}])

```

result ==>

```json
[
  {
    "_id": 2,
    "customer_id": 1,
    "order_date": "2022-03-15",
    "ship_date": "2022-03-18",
    "status": "shipped",
    "total": 25.5
  },
  {
    "_id": 8,
    "customer_id": 3,
    "order_date": "2022-06-15",
    "ship_date": null,
    "status": "pending",
    "total": 35
  }
]
```
