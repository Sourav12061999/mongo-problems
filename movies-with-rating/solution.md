### Queries

1. db.movies.aggregate([ { $group: { _id: "$director", avg_rating: { $avg: "$rating" } } }, { $sort: { avg_rating: -1 } }])

- Expected Output -

```
[
  { _id: 'Nitesh Tiwari', avg_rating: 8.4 },
  { _id: 'Rajkumar Hirani', avg_rating: 8.4 },
  { _id: 'Anurag Kashyap', avg_rating: 8.2 },
  { _id: 'Ashutosh Gowariker', avg_rating: 8.1 },
  { _id: 'S. S. Rajamouli', avg_rating: 8.1 }
]
```
