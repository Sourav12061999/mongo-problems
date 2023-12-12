<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([{$sort:{total:-1}},{$limit:3}]);

```

result ==>

```json
{
  "_id": 1,
  "customer_id": 1,
  "order_date": "2022-03-01",
  "ship_date": "2022-03-05",
  "status": "shipped",
  "total": 50.25
}
```
