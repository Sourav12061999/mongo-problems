<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.orders.aggregate([
  {
    $lookup: {
      from: "buyers",
      localField: "customer_id",
      foreignField: "_id",
      as: "buyer_info"
    }
  },
  {
    $unwind: "$buyer_info"
  }
])

```
