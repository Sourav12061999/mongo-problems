### Query

1.

```json
db.restaurants.find({
  "grades.grade": "A",
  "grades.score": { $gt: 8 }
})
```
