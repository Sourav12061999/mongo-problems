### Queries

1.

```json
db.suppliers.aggregate([
   {$match:{_id:1}},
   {$lookup:{from:"products",localField:"_id",foreignField:"supplier_id",as:"product"}},
   {$unwind:"$product"},
   {$project:{product:1,_id:0}},
   {$lookup:{from:"order_details",localField:"product._id",foreignField:"product_id",as:"order"}},
    {$unwind:"$order"},{$project:{order:1}}
   ]).map(e=>e.order)
```

--> result

```json
[
  {
    "_id": 1,
    "order_id": 1,
    "product_id": 1,
    "quantity": 1,
    "price": 999.99,
    "payment_id": 1,
    "shipper_id": 1
  },
  {
    "_id": 4,
    "order_id": 5,
    "product_id": 5,
    "quantity": 1,
    "price": 1999.99,
    "payment_id": 4,
    "shipper_id": 2
  },
  {
    "_id": 8,
    "order_id": 9,
    "product_id": 5,
    "quantity": 1,
    "price": 1999.99,
    "payment_id": 8,
    "shipper_id": 3
  }
]
```
