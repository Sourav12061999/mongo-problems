### Query

1.

```json
db.restaurants.aggregate([
  {
    $addFields: {
      gradeCount: { $size: "$grades" }
    }
  },
  {
    $match: { gradeCount: { $gt: 5 } }
  },
  {
    $sort: { gradeCount: -1 }
  },
  {
    $limit: 10
  }
]);
```
