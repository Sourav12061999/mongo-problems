### Queries

1.

```json
db.shippers.aggregate([
   {$match:{name:"FedEx"}},
   {$lookup:{from:"order_details",localField:"_id",foreignField:"shipper_id",as:"details"}},
   {$unwind:"$details"},
   {$lookup:{from:"orders",localField:"details.order_id",foreignField:"_id",as:"order"}},
   {$unwind:"$order"},
   {$project:{_id:0,order:1}}
   ])
   .map(e=>e.order)
```

--> result

```json
[
  {
    "_id": 2,
    "customer_id": 1,
    "order_date": "2022-03-15",
    "ship_date": "2022-03-18",
    "status": "shipped",
    "total": 25.5
  },
  {
    "_id": 5,
    "customer_id": 2,
    "order_date": "2022-05-01",
    "ship_date": "2022-05-05",
    "status": "shipped",
    "total": 75
  },
  {
    "_id": 7,
    "customer_id": 3,
    "order_date": "2022-06-01",
    "ship_date": "2022-06-05",
    "status": "shipped",
    "total": 25.5
  },
  {
    "_id": 9,
    "customer_id": 4,
    "order_date": "2022-07-01",
    "ship_date": "2022-07-05",
    "status": "shipped",
    "total": 125.5
  }
]
```
