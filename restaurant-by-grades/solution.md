### Query

1.

```json
db.restaurants.aggregate([
  {
    $unwind: "$grades"
  },
  {
    $sort: { "grades.date": -1 }
  },
  {
    $match: { "grades.grade": "C" }
  }
]);

```
