### Query

1.

```json
db.restaurants.aggregate([
  {
    $group: {
      _id: {
        borough: "$borough",
        name: "$name"
      },
      count: { $sum: 1 }
    }
  },
  {
    $match: { count: { $gte: 2 } }
  },
  {
    $group: {
      _id: "$_id.borough",
      restaurants: { $push: "$_id.name" }
    }
  }
]);

```
