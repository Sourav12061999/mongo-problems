<h1 style="color:#397ce7">Solution Queries:</h1>

1.

```json
db.order_details.aggregate([
  {
    $lookup: {
      from: "orders",
      localField: "order_id",
      foreignField: "_id",
      as: "order"
    }
  },
  {
    $lookup: {
      from: "shippers",
      localField: "shipper_id",
      foreignField: "_id",
      as: "shipper"
    }
  },
  {
    $unwind: "$order"
  },
  {
    $unwind: "$shipper"
  },
  {
    $group: {
      _id: "$shipper_id",
      revenue: { $sum: { $multiply: ["$price", "$quantity"] } }
    }
  },
  {
    $lookup: {
      from: "shippers",
      localField: "_id",
      foreignField: "_id",
      as: "shipper"
    }
  },
  {
    $sort: {
      revenue: -1
    }
  },
  {
    $limit: 1
  },
  {
    $project: {
      _id: 0,
      shipper_id: "$_id",
      shipper_name: { $arrayElemAt: ["$shipper.name", 0] },
      revenue: 1
    }
  }
])

```
