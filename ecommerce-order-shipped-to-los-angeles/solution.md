<h1 style="color:#397ce7">Solution Queries:</h1>

1. Query

```mongodb
db.orders.aggregate([
  {
    $match: {
      "status": "shipped"
    }
  },
  {
    $lookup: {
      from: "buyers",
      localField: "customer_id",
      foreignField: "_id",
      as: "buyerDetails"
    }
  },
  {
    $match: {
      "buyerDetails.address.city": "Los Angeles"
    }
  }
])

```

Response:

```json
[
  {
    "_id": 5,
    "customer_id": 2,
    "order_date": "2022-05-01",
    "ship_date": "2022-05-05",
    "status": "shipped",
    "total": 75,
    "buyerDetails": [
      {
        "_id": 2,
        "name": "Jane Doe",
        "email": "jane@example.com",
        "address": {
          "street": "456 Elm St",
          "city": "Los Angeles",
          "state": "CA",
          "zip": "90001"
        }
      }
    ]
  }
]
```
