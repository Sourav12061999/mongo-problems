<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([{$sort:{ship_date:-1}},{$skip:2},{$limit:1}])

```

result ==>

```json
{
  "_id": 7,
  "customer_id": 3,
  "order_date": "2022-06-01",
  "ship_date": "2022-06-05",
  "status": "shipped",
  "total": 25.5
}
```
