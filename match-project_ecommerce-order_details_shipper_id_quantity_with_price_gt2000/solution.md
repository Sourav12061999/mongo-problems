<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.order_details.aggregate([
  {$match:{price:{$gt:2000}}}, {$project:{shipper_id:1,_id:0,quantity:1}}
  ])

```
