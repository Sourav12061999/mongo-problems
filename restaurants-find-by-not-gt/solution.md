### Query

1. db.restaurants.find( { "grades.score": { $not: { $gt: 10 } } }, { "restaurant_id": 1, "name": 1, "borough": 1, "cuisine": 1 })

- Expected Output -

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d94959b"),
    borough: 'Brooklyn',
    cuisine: 'American',
    name: 'C & C Catering Service',
    restaurant_id: '40357437'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959e"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: '1 East 66Th Street Kitchen',
    restaurant_id: '40359480'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495a2"),
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    name: 'Nordic Delicacies',
    restaurant_id: '40361390'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495ab"),
    borough: 'Brooklyn',
    cuisine: 'Hamburgers',
    name: 'White Castle',
    restaurant_id: '40362344'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495c2"),
    borough: 'Brooklyn',
    cuisine: 'American',
    name: "Sonny'S Heros",
    restaurant_id: '40363744'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495c8"),
    borough: 'Bronx',
    cuisine: 'American',
    name: 'Manhem Club',
    restaurant_id: '40364363'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495d9"),
    borough: 'Staten Island',
    cuisine: 'American',
    name: 'Great Kills Yacht Club',
    restaurant_id: '40364610'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495e4"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'White Horse Tavern',
    restaurant_id: '40364958'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495ea"),
    borough: 'Manhattan',
    cuisine: 'American',
    name: 'Serendipity 3',
    restaurant_id: '40364863'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d9495f0"),
    borough: 'Manhattan',
    cuisine: 'Irish',
    name: "Dorrian'S Red Hand Restaurant",
    restaurant_id: '40365239'
  }
]
```
