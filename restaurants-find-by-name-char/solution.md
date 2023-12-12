### Query

1.  db.restaurants.find( { name: /^Wil/ }, { "restaurant_id": 1, "name": 1, "borough": 1, "cuisine": 1 });

- Expected Output -

```
[
  {
    _id: ObjectId("6447c9678dfeb17a7d949592"),
    borough: 'Brooklyn',
    cuisine: 'Delicatessen',
    name: "Wilken'S Fine Food",
    restaurant_id: '40356483'
  },
  {
    _id: ObjectId("6447c9678dfeb17a7d94959a"),
    borough: 'Bronx',
    cuisine: 'American',
    name: 'Wild Asia',
    restaurant_id: '40357217'
  }
]
```
