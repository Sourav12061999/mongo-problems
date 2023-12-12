### Queries

1.

```json
db.orders.aggregate([
  {$match:{_id:1}},
  {$lookup:{from:"order_details",localField:"_id",foreignField:"order_id",as:"details"}},{$unwind:"$details"},
  {$lookup:{from:"payments",localField:"details.payment_id",foreignField:"_id",as:"payment"}},{$unwind:"$payment"},
  {$project:{"paymentStatus":"$payment.paymentstatus",_id:0}}
  ])
```

    --> result

```json
[
  {
    "paymentStatus": "success"
  }
]
```
