### Query

1.

```json
db.restaurants.aggregate([
  {
    $unwind: "$grades"
  },
  {
    $group: {
      _id: {
        cuisine: "$cuisine",
        restaurant_id: "$restaurant_id"
      },
      averageScore: { $avg: "$grades.score" }
    }
  },
  {
    $sort: {
      "_id.cuisine": 1,
      averageScore: -1
    }
  },
  {
    $group: {
      _id: "$_id.cuisine",
      topRestaurants: { $push: { restaurant_id: "$_id.restaurant_id", averageScore: "$averageScore" } }
    }
  },
  {
    $project: {
      _id: 0,
      cuisine: "$_id",
      topRestaurants: { $slice: ["$topRestaurants", 3] }
    }
  }
]);

```
