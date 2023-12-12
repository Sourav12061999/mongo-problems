### Queries

1.

```json
db.order_details.aggregate([
  {$match:{_id:1}},
  {$lookup:{from:"products",localField:"product_id",foreignField:"_id",as:"product"}},
  {$lookup:{from:"orders",localField:"order_id",foreignField:"_id",as:"order"}},
  {$project:{"product.supplier_id":1,"order.customer_id":1}},
  {$lookup:{from:'suppliers',localField:"product.supplier_id",foreignField:"_id",as:"supplier"}},
  {$lookup:{from:"buyers",localField:"order.customer_id",foreignField:"_id",as:"customer"}},{$unwind:"$supplier"},
  {$unwind:"$customer"},
  {$project:{ "pickup_city": "$supplier.city", "drop_city":"$customer.address.city",_id:0}}
  ])
```

    --> result

```json
[
  {
    "pickup_city": "Cupertino",
    "drop_city": "New York"
  }
]
```
