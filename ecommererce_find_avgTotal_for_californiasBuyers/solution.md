### Queries

1.

```json
db.orders.aggregate([
   {$lookup:{from:"buyers",localField:"customer_id",foreignField:"_id",as:"buyer"}},
   {$unwind:"$buyer"},
   { $match: { "buyer.address.state":'CA' } },
   { $group: { _id: null, avgTotal: { $avg:'$total'  } } },
   {$project:{_id:0,avgTotal: { $trunc: [ "$avgTotal", 0 ] }}}
   ])
```

--> result

```json
{
  "avgTotal": 100
}
```
