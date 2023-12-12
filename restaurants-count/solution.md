### Query

1. db.restaurants.aggregate([{ $group: { _id: "$borough", count: { $sum: 1 } } }])

- Expected Output -

```
[
  { _id: 'Staten Island', count: 9 },
  { _id: 'Manhattan', count: 43 },
  { _id: 'Brooklyn', count: 26 },
  { _id: 'Bronx', count: 7 },
  { _id: 'Queens', count: 15 }
]
```
