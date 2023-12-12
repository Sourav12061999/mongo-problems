<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.buyers.aggregate([
  { $match: { "address.city": "New York" } },
  { $lookup: {
      from: "orders",
      localField: "_id",
      foreignField: "customer_id",
      as: "orders"
    }
  },
  { $unwind: "$orders" },
  { $project: {
      _id: 1,
      name: 1,
      email: 1,
      "address.street": 1,
      "address.city": 1,
      "address.zip": 1,
      "orders.order_date": 1,
      "orders.ship_date": 1,
      "orders.status": 1,
      "orders.total": 1
    }
  }
])
```
