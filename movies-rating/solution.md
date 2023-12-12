### Queries

1. db.movies.aggregate([
  { $group: { _id: null, avgRating: { $avg: "$rating" } } }
]);


- Expected Output -
```
{ "_id": null, "avgRating": 8.24 }
```