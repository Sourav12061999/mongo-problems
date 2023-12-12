<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([{$sort:{ship_date:-1}},{$limit:1}])

```

result ==>

```json
{
  "_id": 10,
  "customer_id": 5,
  "order_date": "2022-08-01",
  "ship_date": "2022-08-05",
  "status": "shipped",
  "total": 75.25
}
```
