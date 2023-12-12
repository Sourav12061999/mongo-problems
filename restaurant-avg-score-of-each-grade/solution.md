### Query

1.

```json
db.restaurants.aggregate([
  {
    $unwind: "$grades"
  },
  {
    $group: {
      _id: "$grades.grade",
      averageScore: { $avg: "$grades.score" }
    }
  }
]);

```
