<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.order_details.aggregate([{$sort:{price:-1}},{$limit:1}])


```

result ==>

```json
{
  "_id": 2,
  "order_id": 2,
  "product_id": 6,
  "quantity": 2,
  "price": 2599.98,
  "payment_id": 2,
  "shipper_id": 2
}
```
