### Queries

1.

```json
db.buyers.aggregate([
  {$match: {_id:1}},
  {$lookup:{from:"orders",localField:"_id",foreignField:"customer_id",as:"items"}},
  {$project:{items:1}},
  {$unwind:"$items"},
  {$lookup:{from:"order_details",localField:"items._id",foreignField:"order_id",as:"orderDtl"}},{$project:{orderDtl:1}},
  {$unwind:"$orderDtl"},
  {$lookup:{from:"payments",localField:"orderDtl.payment_id",foreignField:"_id",as:"payment"}},{$unwind:"$payment"},
  {$group:{_id:"$payment.paymentMethod"}}
  ])
  .map(e=>e._id)
```

    --> result

```json
["UPI", "Debit Card", "Cradit Card"]
```
