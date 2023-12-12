### Queries

1.

```json
db.orders.aggregate([ { $group: { _id: "$customer_id", total_amount: { $sum: "$total" } } }, { $sort: { total_amount: -1 } }, { $limit: 3 }, { $lookup: { from: "buyers", localField: "_id", foreignField: "_id", as: "customer_info" } }, { $unwind: "$customer_info" }, { $project: { customer_id: "$customer_info._id", name: "$customer_info.name", total_amount: 1 } } ])
```
