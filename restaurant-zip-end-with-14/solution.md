### Query

1.

```json
db.restaurants.aggregate([
  {
    $match: { "address.zipcode": /14$/ }
  },
  {
    $group: {
      _id: "$cuisine",
      count: { $sum: 1 }
    }
  },
  {
    $sort: { count: -1 }
  },
  {
    $limit: 3
  }
])
```
