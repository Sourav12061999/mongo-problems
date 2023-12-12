### Queries

1.

```json
db.payments.aggregate([
   {$match:{paymentstatus:"pending"}},
   {$lookup:{from:"order_details",localField:"orderdtl_id",foreignField:"_id",as:"details"}},{$unwind:"$details"},
   {$lookup:{from:"orders",localField:"details.order_id",foreignField:"_id",as:"order"}},
   {$unwind:"$order"},
   {$project:{_id:0,"ship_date":"$order.ship_date","order_date":"$order.order_date"}}
   ])
```

--> result

```json
[
  {
    "ship_date": "2022-06-05",
    "order_date": "2022-06-01"
  }
]
```
