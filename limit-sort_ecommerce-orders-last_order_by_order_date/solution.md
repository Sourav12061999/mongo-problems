<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([{$sort:{order_date:-1}},{$limit:1}])

```

result ==>

```json
{
  "_id": 11,
  "customer_id": 5,
  "order_date": "2022-08-15",
  "ship_date": null,
  "status": "pending",
  "total": 50
}
```
