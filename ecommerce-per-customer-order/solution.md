### Queries

1.

```json
db.orders.aggregate([
  {
    $lookup: {
      from: "buyers",
      localField: "customer_id",
      foreignField: "_id",
      as: "customer"
    }
  },
  { $unwind: "$customer" },
  { $group: { _id: "$customer.name", order_count: { $sum: 1 } } }
])
```
