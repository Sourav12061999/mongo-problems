<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.order_details.aggregate([{$sort:{price:1}},{$limit:1}])


```

result ==>

```json
{
  "_id": 10,
  "order_id": 10,
  "product_id": 7,
  "quantity": 1,
  "price": 149.99,
  "payment_id": 10,
  "shipper_id": 1
}
```
