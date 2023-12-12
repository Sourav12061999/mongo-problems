### Queries

1.

```json
db.orders.aggregate([
  {$match:{_id:1}},
  {$lookup:{from:"order_details",localField:"_id",foreignField:"order_id",as:"details"}},{$unwind:"$details"},
  {$lookup:{from:"shippers",localField:"details.shipper_id",foreignField:"_id",as:"shipper"}},{$unwind:"$shipper"},
  {$project:{"shiperName":"$shipper.name",_id:0}}
  ])
```

    --> result

```json
[
  {
    "shiperName": "UPS"
  }
]
```
